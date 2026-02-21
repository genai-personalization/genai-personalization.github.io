---
permalink: /GenAIRecP2026
title: "Third Workshop on Generative AI for Recommender Systems and Personalization <br>(2026)"
excerpt: Thursday Feb. 26, 2026, Boise, Idaho, USA <br> Held in conjunction with <a href="https://wsdm-conference.org/2026/">WSDM 2026</a>
browser-title: "GenAIRecP 2026"
masthead-title: "GenAIRecP 2026"
masthead-subtitle: "@WSDM 2026"
masthead-url: "/"
layout: splash
author_profile: false
header:
    overlay_color: "#000"
    overlay_filter: "0.5"
    overlay_image: /assets/images/GenAIBanner.PNG
navigation:
  - title: "CfP"
    url: /GenAIRecP2026/call-for-papers
  - title: "Schedule"
    url: /GenAIRecP2026#schedule
  - title: "Keynotes"
    url: /GenAIRecP2026#keynote-speakers
  # - title: "Panelists"
  #   url: /GenAIRecP2026#panelists
  - title: "Organization"
    url: /GenAIRecP2026#organizers

keynote:
    - image_path: /assets/images/GenAIRecP2026/chirag.png
      alt: "Chirag Shah"
      title: "Chirag Shah"
      excerpt: |
        ***University of Washington*** <br>
        **Beyond the Personalization-Privacy Pareto: Can AI Agents Break the Tradeoff?**

      abstract: >
        The tension between personalization and privacy has long been treated as an immutable tradeoff—more of one necessarily means less of the other. But as we move from reactive AI systems to proactive AI agents that act on our behalf, this calculus may be shifting. This keynote examines whether agentic AI architectures—with their capacity for local reasoning, on-device memory, and user-controlled delegation—offer a path beyond the Pareto frontier. I explore emerging paradigms where agents can deliver deeply personalized experiences while minimizing data exposure, and discuss the technical, ethical, and governance challenges that remain. The talk concludes with a research agenda for building AI agents that treat privacy not as a constraint on personalization, but as a design principle that enables it.

      bio: >
        Chirag Shah is a Professor of Information and Computer Science at University of Washington (UW) in Seattle. He is the Founding Director for InfoSeeking Lab and Founding Co-Director of Center for Responsibility in AI Systems & Experiences (RAISE). His research focuses on building, auditing, and correcting agentic information access systems. Shah is a Distinguished Member of ACM as well as ASIS&T, and a Senior Member of IEEE. He has published nearly 200 peer-reviewed articles and authored ten books, including textbooks on data science and machine learning. His new book is called 'Agent Nation: How Autonomous AI Is Rewriting the Rules of Society—and What We Can Do About It'—coming out this spring.

      spaces: true

    - image_path: /assets/images/GenAIRecP2026/Yinglong.jpg
      alt: "Yinglong Xia"
      title: "Yinglong Xia"
      excerpt: |
        ***Meta*** <br>
        **The Graph Trilogy: Unlocking Personalization at Scale**

      abstract: >
        This talk will present the graph trilogy techniques to overcome the persistent personalization gap in large-scale recommendation systems, arguing that large AI models alone cannot solve challenge of effectively modeling billions of unique user preferences. The core solution involves establishing a Context Graph to capture richer, multi-hop, and structural relationships, thereby transforming traditional engagement data into actionable intelligence for discovery and diversity. To effectively leverage this structural information, the presentation presents co-modeling the user-centric heterogeneous graph with a ranking model. Furthermore, to scale personalization by injecting this complex user knowledge into LLMs, the paper introduces the structural mixture of residual experts that utilizes a structural MoE to exponentially boost model capacity and expressive power while maintaining the parameter efficiency required for industrial-scale deployment.

      bio: >
        Yinglong Xia is an Applied Research Scientist at Meta Recommendation System (MRS), Meta Platforms, where he focuses on advancing research and development in large-scale recommendation systems and knowledge-driven AI, driving innovation and delivering impactful solutions that enhance Meta's products and user experiences. Prior to that, he was a chief architect at Huawei US on the Enterprise AI and Research Staff Member at IBM Watson Research Center. He published 100+ technical papers and filed 40+ patents, serving as an AE for IEEE TBD, an ADS area chair at KDD 2025, an industry co-chair of CIKM 2024 and WSDM 2026.

      spaces: true

    - image_path: /assets/images/GenAIRecP2026/Meng.jpg
      alt: "Meng Jiang"
      title: "Meng Jiang"
      excerpt: |
        ***University of Notre Dame*** <br>
        **What Does It Mean to Personalize a Language Model? Insights from RecSys to LLMs**

      abstract: >
        Personalization has been a foundational concept in recommender systems (RecSys) since the emergence of collaborative filtering, where models adapt predictions to individual users based on historical interactions. This paradigm has rapidly extended to large language models (LLMs), giving rise to personalized LLMs that tailor textual responses, reasoning styles, and interaction behaviors to individual users. Beyond improved user experience, personalization in LLMs opens new opportunities related to data privacy, user control, and model ownership. This shift raises fundamental questions about how personalization should be defined, implemented, and evaluated in the context of general-purpose language models. In this keynote, I trace the evolution of personalization from classical RecSys to personalized LLMs, highlighting both conceptual continuities and critical departures between these paradigms. I then introduce emerging technical approaches (particularly parameter-efficient adaptation methods) that enable LLMs to incorporate user-specific signals at scale. Finally, I present a recent study to link the two technologies to answer if personalized LLMs are already strong recommender systems.

      bio: >
        Meng Jiang is a Frank M. Freimann Collegiate Associate Professor of Computer Science and Engineering at the University of Notre Dame. He is appointed as the Director of Foundation Models at the Lucy Family Institute for Data and Society as well as the Program Chair of ND-IBM Tech Ethics Lab. His research interests are data mining, machine learning, and natural language processing for AI applications in science, engineering, social media, education, and healthcare. His recent projects focus on knowledge augmentation, instruction tuning, multi-objective alignment, reasoning and verification, personalization, and machine unlearning. He has delivered 15 conference tutorials and organized ten workshops on these topics. He has received five best paper or outstanding paper awards and the NSF CAREER award.

      spaces: true

    - image_path: /assets/images/GenAIRecP2026/nathan.jpg
      alt: "Nathan Kallus"
      title: "Nathan Kallus"
      excerpt: |
        ***Cornell Tech, Netflix*** <br>
        **LLM Post-Training and Reasoning via Efficient Value-Based RL**

      abstract: >
        Reinforcement learning (RL) has a newfound killer application in post-training LLMs pre-trained to predict next token to adapt to tasks like instruction following, math-problem solving, and generating content or recommendations that maximize user outcomes. But are the same RL algorithms that animated robots and conquered Atari the right ones to post-train LLMs? In this talk I will present new value-based algorithms for post-training and for scaling test-time compute that leverage both the unique structure of autoregressive LLMs and recent advances on increasing efficiency by changing the Q-learning loss function. I will show how (and argue why) these new algorithms achieve state-of-the-art performance on frontier math reasoning tasks with smaller models and at a fraction of test-time FLOPs.

      bio: >
        Nathan Kallus is an Associate Professor at the Cornell Tech campus of Cornell University in NYC and Director of Machine Learning and Inference Research at Netflix. Nathan's research interests include causal machine learning, sequential and dynamic decision making, optimization under uncertainty, and algorithmic fairness.

      spaces: true

# panelists:
#     - image_path: /assets/images/GenAIBanner.PNG
#       alt: "Panelist 1"
#       excerpt: >
#         **TBD**<br>
#         TBD Affiliation
#       bio: >
#         Bio will be updated closer to the workshop date.
#
#     - image_path: /assets/images/GenAIBanner.PNG
#       alt: "Panelist 2"
#       excerpt: >
#         **TBD**<br>
#         TBD Affiliation
#       bio: >
#         Bio will be updated closer to the workshop date.

organizers:
    - image_path: /assets/images/GenAIRecP2026/Narges.jpg
      alt: "Narges Tabari"
      excerpt: >
        **Narges Tabari**<br>
        AWS AI Labs
      bio: >
        Narges Tabari is an Applied Scientist working at AWS AI Labs. She received her PhD in 2018 in Computer Science at the University of North Carolina. She mainly wroks towards applications of NLP, from sentiment analysis, emotion detection, summarization, text generation, and intersection of NLP with recommender systems and personalization. Before joining Amazon, she was a Research Scientist at the University of Virginia and an NLP Engineer at Genentech. She has served as Session Chair for NAACL 2022 Industry Track, and has extensive experience reviewing for conferences such as NAACL, AAAI, and ACL.
        
    - image_path: /assets/images/GenAIRecP2026/Aniket.JPG
      alt: "Aniket Deshmukh"
      excerpt: >
        **Aniket Deshmukh**<br>
        Databricks
      bio: >
        Aniket is an AI researcher at Databricks. Aniket was an Applied Scientist at AWS AI Labs, focusing on recommendation systems and large language models. Previously, as a Senior Applied Scientist at Microsoft AI and Research, he contributed to Microsoft Advertising by working on multimedia ads, smart campaigns, and auto-bidding projects. Aniket earned his PhD in Electrical and Computer Engineering from the University of Michigan, Ann Arbor, focusing on domain generalization and reinforcement learning. He is an active contributor to the academic community, regularly reviewing for conferences such as NeurIPS, ICML, CVPR, AISTATS, and JMLR, and has been recognized as a top reviewer at NeurIPS in 2021 and 2023, as well as AISTATS in 2022. Aniket has experience in organizing workshops at conferences like ICLR and WWW.

    - image_path: /assets/images/GenAIRecP2026/Wang.jpg
      alt: "Wang-Cheng Kang"
      excerpt: >
        **Wang-Cheng Kang**<br>
        Google DeepMind
      bio: >
        Dr. Wang-Cheng Kang is a Staff Research Engineer at Google DeepMind, working on LLM/GenAI for RecSys and LLM data efficiency. He held a PhD in Computer Science from UC San Diego, and interned at Adobe Research, Pinterest Labs, and Google Brain, focusing on recommender systems. He received RecSys'17 Best Paper Runner-up, and proposed SASRec, the first Transformer-based recommendation method.

    - image_path: /assets/images/GenAIRecP2026/Neil_professional_snap_aug22.jpg
      alt: "Neil Shah"
      excerpt: >
        **Neil Shah**<br>
        Snap Research
      bio: >
        Dr. Neil Shah is a Principal Scientist at Snapchat. His research focuses on large-scale user representation learning, recommender systems and efficient ML. His work has resulted in 70+ refereed publications at top data mining and machine learning venues. He has also served as an organizer across multiple venues including KDD, WSDM, SDM, ICWSM, ASONAM and more, and received multiple best paper awards (KDD, CHI), departmental rising star awards (NCSU), and outstanding service and reviewer awards (NeurIPS, WSDM).

    - image_path: /assets/images/GenAIRecP2026/Julian.jpg
      alt: "Julian McAuley"
      excerpt: >
        **Julian McAuley**<br>
        University of California, San Diego
      bio: >
        Julian McAuley has been a professor in the Computer Science Department at the University of California, San Diego since 2014. Previously he was a postdoctoral scholar at Stanford University after receiving his PhD from the Australian National University in 2011. His research is concerned with developing predictive models of human behavior using large volumes of online activity data. He has organized a large number of workshops, including workshops on recommendation, e-commerce, and natural language processing.

    - image_path: /assets/images/GenAIRecP2026/caverlee.jpeg
      alt: "James Caverlee"
      excerpt: >
        **James Caverlee**<br>
        Texas A&M University
      bio: >
        James Caverlee received his Ph.D. in Computer Science from Georgia Tech in 2007, co-advised by Ling Liu (CS) and Bill Rouse (ISYE). Before that, he earned two M.S. degrees from Stanford University: one in Computer Science in 2001 and one in Engineering-Economic Systems & Operations Research in 2000. His undergraduate degree is a B.A. in Economics (magna cum laude) from Duke University in 1996. James Caverlee joined the faculty at Texas A&M in 2007. He spent most of his sabbatical in 2015 at Google as a Visiting Scientist in Ed Chi's group. He has been honored to receive an NSF CAREER award, DARPA Young Faculty award, a AFOSR Young Investigator award, as well as several teaching awards.
        
    - image_path: /assets/images/GenAIRecP2026/GeorgeKarypis.jpeg
      alt: "George Karypis"
      excerpt: >
        **George Karypis**<br>
        University of Minnesota 
      bio: >
        Dr. George Karypis is a Senior Principal Scientist at AWS AI and a Distinguished McKnight University Professor and William Norris Chair in Large Scale Computing at the Department of Computer Science & Engineering at the University of Minnesota. His research interests span the areas of data mining, machine learning, high performance computing, information retrieval, collaborative filtering, bioinformatics, cheminformatics, and scientific computing. He has coauthored over 350 papers and two books.
        
---

<script>
if (!sessionStorage.getItem('timezone')) {
  var tz = jstz.determine() || 'UTC';
  sessionStorage.setItem('timezone', tz.name());
}
var currTz = sessionStorage.getItem('timezone');
var startTime = moment("2026-02-26T08:45:00Z");
var tzTime = startTime.tz(currTz)
</script>

# Overview
Personalization is key in understanding user behavior and has been a main focus in the fields of knowledge discovery and information retrieval. Building personalized recommender systems is especially important now due to the vast amount of user-generated textual content, which offers deep insights into user preferences. The recent advancements in Large Language Models (LLMs) have significantly impacted research areas, mainly in Natural Language Processing and Knowledge Discovery, giving these models the ability to handle complex tasks and learn context.

However, the use of generative models and user-generated text for personalized systems and recommendation is relatively new and has shown some promising results. This workshop is designed to bridge the research gap in these fields and explore personalized applications and recommender systems. We aim to fully leverage generative models to develop AI systems that are not only accurate but also focused on meeting individual user needs. Building upon the momentum of previous successful forums, this workshop seeks to engage a diverse audience from academia and industry, fostering a dialogue that incorporates fresh insights from key stakeholders in the field. 

# Call for papers
We will welcome papers that leverage generative models with a goal of recommendation and personalization on several topics including but not limited to those mentioned in [CFP](/GenAIRecP2026/call-for-papers). Papers can be submitted via [OpenReview](https://openreview.net/group?id=WDSM/2026/Workshop/GenAIRecP). Submissions may be 2-8 pages (excluding references and supplementary materials). 

## Information for the day of the workshop

**Workshop at WSDM 2026**    
- Submission deadline: ~~November 21, 2025~~ November 28, 2025
- Author notifications: December 18, 2025
- Meeting: February 26, 2026

# Schedule

| Time (MST) | Agenda |
| ----------------- | ------------ |
| **8:55 - 9:00am** | **Opening remarks** |
| **9:00 - 9:45am** | **[Keynote by Dr. Meng Jiang](#Meng+Jiang) (45 min)** |
| **9:45 - 10:30am** | **[Keynote by Dr. Yinglong Xia](#Yinglong+Xia) (45 min)** |
| **10:30 - 11:00am** | **Coffee Break (30 min)** |
| **11:00 - 11:45am** | **Oral Session 1 (45 min)** - Paper Authors<br>- AGP: Auto-Guided Prompt Refinement for Personalized Reranking in Recommender Systems<br>- InsertRank: LLMs can Reason over BM25 Scores to Improve Listwise Reranking<br>- Selective LLM-Guided Regularization for Enhancing Recommendation Models |
| **11:45am - 12:30pm** | **[Keynote by Dr. Chirag Shah](#Chirag+Shah) (45 min)** |
| **12:30 - 1:45pm** | **Lunch (75 min)** |
| **1:45 - 2:30pm** | **[Keynote by Dr. Nathan Kallus](#Nathan+Kallus) (45 min)** |
| **2:30 - 3:30pm** | **Oral Session 2 (60 min)** - Paper Authors<br>- Joint Evaluation: A Human+LLM+Multi-Agents Collaborative Framework for Comprehensive AI Safety<br>- Multi-Agent Video Recommenders: Evolution, Patterns and Open Challenges<br>- Large-Scale Retrieval for the LinkedIn Feed using Causal Language Models<br>- Agentic Orchestration for Adaptive Educational Recommendations: A Multi-Agent LLM Framework for Personalized Learning Pathways |
| **3:30 - 4:00pm** | **Coffee Break (30 min)** |
| **4:00 - 4:20pm** | **[Invited Talk by Liam Collins] (20 min)**<br>Sequential Data Augmentation for Generative Recommendation |
| **4:20 - 4:40pm** | **[Invited Talk by Chengyi Liu] (20 min)**<br>Continuous Time Discrete-space Diffusion Model for Recommendation |
| **4:40 - 4:50pm** | **Closing remarks** |

<div class="small">
{{ schedule | markdownify }}
</div>

# Keynote Speakers
{% include feature_row id="keynote" type="left" %}

<!-- # Panelists
{% include feature_row id="panelists" %} -->

# Accepted Papers
<ul>
{% for pubitem in site.data.papers2026 %}
    <li> {{ pubitem.title | markdownify | remove: '<p>' | remove: '</p>' | strip }} <br>
    <div class="small">
    <i> {{ pubitem.authors | markdownify | remove: '<p>' | remove: '</p>' | strip }} </i> 
    </div>
    {% if pubitem.abstract %} 
    <a class="btn btn--small btn--info collapsible">Abstract</a> 
    <div class="btn-content small">
        <b>Abstract</b>: {{ pubitem.abstract }}
    </div>
    {% endif %}
    {% if pubitem.PDF %} <a href="{{ pubitem.PDF }}" class="btn btn--small btn--info">PDF</a>{% endif %}
    {% if pubitem.code %} <a href="{{ pubitem.code }}" class="btn btn--small btn--info">
    {% if pubitem.new_dataset %} Code & Datasets {% else %} Code {% endif %} </a>{% endif %}
    </li>
{% endfor %}
</ul>

# Organizers
{% include feature_row id="organizers" %}

# Program Committee
<div class="small row-two-columns">
<div class="column-half">
<ul>
{% for people in site.data.pc-members2026 limit:11 %}
<li>{{ people | markdownify | remove: '<p>' | remove: '</p>' | strip }} </li>
{% endfor %}
</ul>
</div>
<div class="column-half">
<ul>
{% for people in site.data.pc-members2026 offset:11 %}
<li>{{ people | markdownify | remove: '<p>' | remove: '</p>' | strip }} </li>
{% endfor %}
</ul>
</div>
</div>

<script>
    var coll = document.getElementsByClassName("collapsible");
    var i;

    for (i = 0; i < coll.length; i++) {
    coll[i].addEventListener("click", function() {
        this.classList.toggle("active");
        var content = this.nextElementSibling;
        if (content.style.display === "block") {
        content.style.display = "none";
        } else {
        content.style.display = "block";
        }
    });
    }
</script>
