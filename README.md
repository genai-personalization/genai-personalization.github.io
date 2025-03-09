# GenAI Personalization Workshop Website

This repository hosts the official website for the GenAI Personalization Workshop series, which focuses on the intersection of Generative AI and Personalization technologies.

## About the Website

This website is based on [Jekyll](https://jekyllrb.com) and [minimal-mistakes](https://mmistakes.github.io/minimal-mistakes/) theme. It serves as the central hub for information about the annual GenAI Personalization Workshop, including:

- Call for papers
- Workshop schedules
- Keynote speakers
- Panelists
- Accepted papers
- Organizing committee

## Website Structure

- **Configuration**: Main website configurations can be found in `_config.yml`
- **Paper Data**: 
  - Current year's accepted papers data is in `_data/papers.yml`
  - Year-specific paper data is stored in files like `_data/papers2024.yml`
- **Pages**: 
  - Workshop pages are organized by year in the `pages/` directory
  - Each year has its own subdirectory (e.g., `pages/GenAIRecP2024/`)
- **Assets**: 
  - Images, PDFs, and other assets are stored in the `assets/` directory
  - Year-specific assets are organized in subdirectories (e.g., `assets/images/GenAIRecP2024/`)

## Yearly Updates

The website is designed to support annual iterations of the workshop. Each year follows the naming convention `GenAIRecP{YEAR}` (e.g., GenAIRecP2024, GenAIRecP2025).

When creating a new year's workshop:

1. Create a new directory under `pages/` with the appropriate year (e.g., `pages/GenAIRecP2025/`)
2. Create a new data file for papers (e.g., `_data/papers2025.yml`)
3. Update the main index.html redirect to point to the current year
4. Update navigation links in `_data/navigation.yml` as needed

## Local Development

To run the website locally:

1. Install Jekyll and Ruby dependencies
2. Run `bundle exec jekyll serve`
3. Access the site at `http://localhost:4000`

## Contributing

Contributions to improve the website are welcome. Please submit a pull request with your proposed changes.

