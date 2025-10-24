## GenAI Personalization Website - Codebase Overview

### What this site is
- **Framework**: Jekyll using the Minimal Mistakes theme
- **Purpose**: Annual workshop site with per-year landing pages, CfP, schedule, speakers, accepted papers, organizers, and PC list
- **Current redirect**: `index.html` points to the current year (`/GenAIRecP2025`)

### Global configuration and theme
- **_config.yml**: Site-wide settings, plugins, pagination, theme skin, analytics, and includes `_pages`
- **Theme assets**: `_layouts`, `_includes`, `_sass`, and `assets/js|css` come from Minimal Mistakes with light customization
- **Head scripts**: Moment + timezone detection used by year pages for localizing times

### Navigation and UI text
- **_data/navigation.yml**: Top nav; currently only "Current Edition" → `/`
- **_data/ui-text.yml**: Theme locale strings (no year-specific edits required)

### Year-specific content model
Each year has:
- A landing page at `pages/GenAIRecP{YEAR}/index.md` with front matter blocks for:
  - `permalink`, titles, `layout: splash`, masthead, and `navigation` (anchors and CfP link)
  - `keynote` array for featured speakers (rendered with `{% include feature_row %}`)
  - `panelists` array (rendered with `{% include feature_row %}`)
  - `organizers` array (rendered with `{% include feature_row %}`)
  - Schedule table in markdown, and timezone snippet using Moment/jstz
  - Accepted papers rendered from a year-specific data file
- A CfP page at `pages/GenAIRecP{YEAR}/call-for-papers.md`
- Year assets under:
  - Images: `assets/images/GenAIRecP{YEAR}/`
  - Papers (PDFs): `assets/papers/GenAIRecP{YEAR}/`
- Data files under `_data/`:
  - Accepted papers: `_data/papers{YEAR}.yml`
  - Program committee: `_data/pc-members{YEAR}.yml`

### 2024 specifics
- Pages: `pages/GenAIRecP2024/index.md`, `pages/GenAIRecP2024/call-for-papers.md`
- Data: `_data/papers2024.yml`, `_data/pc-members2024.yml`
- Assets: images in `assets/images/GenAIRecP2024/`; PDFs in `assets/papers/GenAIRecP2024/`
- Index renders accepted papers by iterating `site.data.papers2024` and shows PC by iterating `site.data.pc-members2024`

### 2025 specifics
- Pages: `pages/GenAIRecP2025/index.md`, `pages/GenAIRecP2025/call-for-papers.md`
- Data: `_data/papers2025.yml`, `_data/pc-members2025.yml`
- Assets: images in `assets/images/GenAIRecP2025/`; PDFs in `assets/papers/GenAIRecP2025/`
- Index renders accepted papers by iterating `site.data.papers2025` (supports optional `award` flag)

### Routing and landing behavior
- `index.html` uses a meta refresh + canonical link to redirect to the current year path (presently `/GenAIRecP2025`)
- Year pages provide internal navigation via their front matter `navigation` block (anchors: schedule, keynotes, panelists, organizers)

### How accepted papers render
- Year index loops over `site.data.papers{YEAR}` and displays:
  - `title`, `authors`
  - Optional `abstract` via collapsible panel
  - Optional `PDF` link and `code` link; `new_dataset` toggles button label
  - 2025 variant supports optional `award` shown as a badge

### How speakers and organizers render
- Front matter arrays (`keynote`, `panelists`, `organizers`) drive `{% include feature_row %}` components from Minimal Mistakes
- Each entry supports: `image_path`, `alt`, `title` or `excerpt` with rich HTML/markdown, and optional `bio`

### Program Committee rendering
- Year index splits `_data/pc-members{YEAR}.yml` into two columns using Liquid with `limit` and `offset`

### Files to duplicate/update for a new year (2026)
1. Create pages
   - Copy `pages/GenAIRecP2025/` → `pages/GenAIRecP2026/`
   - Update front matter: `permalink: /GenAIRecP2026`, titles, dates, location, `navigation` URLs, schedule table, and speaker/panelist/organizer arrays
2. Create data files
   - `_data/papers2026.yml` (accepted papers)
   - `_data/pc-members2026.yml` (program committee)
3. Add assets
   - `assets/images/GenAIRecP2026/` (headshots, banners)
   - `assets/papers/GenAIRecP2026/` (PDFs); update `PDF` paths in `_data/papers2026.yml`
4. Update landing redirect
   - Edit `index.html` to `URL=/GenAIRecP2026` and canonical href accordingly
5. Update navigation (optional)
   - `_data/navigation.yml` if you want explicit links to prior editions or sections
6. Verify includes and scripts
   - Ensure head scripts in `_config.yml` remain (Moment/jstz) for timezone display

### Quick checklist for 2026
- [ ] `pages/GenAIRecP2026/index.md` created and content updated
- [ ] `pages/GenAIRecP2026/call-for-papers.md` created and content updated
- [ ] `_data/papers2026.yml` added and populated
- [ ] `_data/pc-members2026.yml` added and populated
- [ ] `assets/images/GenAIRecP2026/` created with images referenced by pages
- [ ] `assets/papers/GenAIRecP2026/` created and PDFs uploaded; data file links updated
- [ ] `index.html` redirect points to `/GenAIRecP2026`
- [ ] Update `_data/navigation.yml` if adding menu items for 2026

### Local development
- Run with `bundle exec jekyll serve` and visit `http://localhost:4000`

### Notes and conventions
- Year key is `GenAIRecP{YEAR}` everywhere (paths, permalinks, assets, data filenames)
- Keep image and PDF paths absolute from site root (e.g., `/assets/images/...`)
- For long bios/abstracts, prefer using YAML `|` and `>` block scalars for readability
