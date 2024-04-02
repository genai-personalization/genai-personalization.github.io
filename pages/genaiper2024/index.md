---
permalink: /genaiper2024
title: "Workshop on Generative AI for Recommender Systems and Personalization <br>(2024)"
excerpt: Monday Aug. 26, 2024, 8am - 12pm <br> TBD, TBD <br> Held in conjunction with <a href="https://kdd.org/kdd2024/">KDD 2024</a>
browser-title: "GenAIPer 2024"
masthead-title: "GenAIPer 2024"
masthead-subtitle: "@KDD 2024"
masthead-url: "/"
layout: splash
author_profile: false
header:
    overlay_color: "#000"
    overlay_filter: "0.5"
    overlay_image: /assets/images/glb-bg.jpg
navigation:
  - title: "CfP"
    url: /genaiper2024/call-for-papers
  - title: "Schedule"
    url: /genaiper2024#schedule
  - title: "Keynotes"
    url: /genaiper2024#keynote-speakers
  - title: "Panelists"
    url: /genaiper2024#panelists
  - title: "Organization"
    url: /genaiper2024#organizers
  - title: "Past Editions"
    url: /all-editions

keynote: 
    - image_path: /assets/images/genaiper2024/Aniket.JPG
      alt: "Aniket Deshmukh"
      title: "Aniket Deshmukh"
      excerpt: |
        ***AWS AI Labs*** <br>
        **Title of the talk**

      abstract: >
        Abstract.
      
      bio: >
        Aniket is an Applied Scientist at AWS AI Labs, focusing on recommendation systems and large language models. Previously, as a Senior Applied Scientist at Microsoft AI and Research, he contributed to Microsoft Advertising by working on multimedia ads, smart campaigns, and auto-bidding projects. Aniket earned his PhD in Electrical and Computer Engineering from the University of Michigan, Ann Arbor, focusing on domain generalization and reinforcement learning. He is an active contributor to the academic community, regularly reviewing for conferences such as NeurIPS, ICML, CVPR, AISTATS, and JMLR, and has been recognized as a top reviewer at NeurIPS in 2021 and 2023, as well as AISTATS in 2022. Aniket has experience in organizing workshops at conferences like ICLR and WWW.

      spaces: true


panelists:
    - image_path: /assets/images/genaiper2024/Aniket.JPG
      alt: "Aniket Deshmukh"
      excerpt: >
        **Aniket Deshmukh**<br>
        AWS AI Labs
      bio: >
        Aniket is an Applied Scientist at AWS AI Labs, focusing on recommendation systems and large language models. Previously, as a Senior Applied Scientist at Microsoft AI and Research, he contributed to Microsoft Advertising by working on multimedia ads, smart campaigns, and auto-bidding projects. Aniket earned his PhD in Electrical and Computer Engineering from the University of Michigan, Ann Arbor, focusing on domain generalization and reinforcement learning. He is an active contributor to the academic community, regularly reviewing for conferences such as NeurIPS, ICML, CVPR, AISTATS, and JMLR, and has been recognized as a top reviewer at NeurIPS in 2021 and 2023, as well as AISTATS in 2022. Aniket has experience in organizing workshops at conferences like ICLR and WWW.
 
---


<!-- <div class="notice--info">
  <!-- <h4 class="no_toc">Notice Headline:</h4> ~~>
  {{ notice-text | markdownify }}
</div> -->

<script>
if (!sessionStorage.getItem('timezone')) {
  var tz = jstz.determine() || 'UTC';
  sessionStorage.setItem('timezone', tz.name());
}
var currTz = sessionStorage.getItem('timezone');
var startTime = moment("2024-04-26T08:45:00Z");
var tzTime = startTime.tz(currTz)
</script>

# Overview
Personalization is key in understanding user behavior and has been a main focus in the fields of knowledge discovery and information retrieval. Building personalized recommender systems is especially important now due to the vast amount of user-generated textual content, which offers deep insights into user preferences. The recent advancements in Large Language Models (LLMs) have significantly impacted research areas, mainly in Natural Language Processing and Knowledge Discovery, giving these models the ability to handle complex tasks and learn context.

However, the use of generative models and user-generated text for personalized systems and recommendation is relatively new and has shown some promising results. This workshop is designed to bridge the research gap in these fields and explore personalized applications and recommender systems. We aim to fully leverage generative models to develop AI systems that are not only accurate but also focused on meeting individual user needs. Building upon the momentum of previous successful forums, this workshop seeks to engage a diverse audience from academia and industry, fostering a dialogue that incorporates fresh insights and anticipates over 50 attendees, including key stakeholders in the field. 

## Information for the day of the workshop

**Workshop at KDD2024**    
Submission deadline: 28 May 2024

Author notifications: 28 June 2024

Meeting: 26 August 2024

# Schedule

We have a full-day program from <u>8am to 5pm on Sunday (Aug. 6)</u> at ***Grand Ballroom B***. 

| Time (PDT) | Agenda |
| ----------------- | ------------ |
| **8:00-8:10am**    | **Opening remarks** |
| **8:10-8:50am**    | **[Keynote by Aniket Deshmukh](#Aniket+Deshmukh) (40 min)**: <br> XYZ |
| **8:50-9:30am**    | **[Keynote by Aniket Deshmukh](#Aniket+Deshmukh) (40 min)**: <br> XYZ |
| **9:30-10:30am**    | **Coffee Break/Poster Session** |
| **10:30-11:00am**    | **[Keynote by Aniket Deshmukh](#Aniket+Deshmukh) (30 min)**: <br> XYZ |
| **11:00-12:00pm**    | **[Panel Discussion](#panelists) (60 min)**<br>**Moderator**:Aniket Deshmukh<br>**Panelists**: Aniket Deshmukh, Aniket Deshmukh, Aniket Deshmukh|
| **12:00-12:10pm**    | **Closing Remarks** |

<div class="small">
{{ schedule | markdownify }}
</div>


# Keynote Speakers
{% include feature_row id="keynote" type="left" %}

# Panelists
{% include feature_row id="panelists" %}

# Accepted Papers
<ul>
{% for pubitem in site.data.papers2024 %}
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
Please contact us through <a target="_blank" href="https://mailhide.io/e/5RV52Tlm">this email address</a> if you have any questions.

{% capture organizers %}
A list of organizers can also be found [here](https://airtable.com/shrwvG9wYqjrbXq0s/tblLXlCDQlpCBK6lR?backgroundColor=purple).
{% endcapture %}

<div class="small">
{{ organizers | markdownify }}
</div>

<style>
    #organizer-wrap { width: 100%; height: 750; padding: 0; overflow: hidden; }
    #organizer-frame { width: 107%; height: 750; background: transparent; border: 1px solid #ccc; }
    #organizer-frame {
        -ms-zoom: 0.93;
        -moz-transform: scale(0.93);
        -moz-transform-origin: 0 0;
        -o-transform: scale(0.93);
        -o-transform-origin: 0 0;
        -webkit-transform: scale(0.93);
        -webkit-transform-origin: 0 0;
    }
</style>
<div id="organizer-wrap">
<iframe id="organizer-frame" class="airtable-embed" src="https://airtable.com/embed/shrwvG9wYqjrbXq0s?backgroundColor=purple" frameborder="0" onmousewheel="" height="750" style="background: transparent; border: 1px solid #ccc;"></iframe>
</div>

<!-- <iframe class="airtable-embed" src="https://airtable.com/embed/shrwvG9wYqjrbXq0s?backgroundColor=purple" frameborder="0" onmousewheel="" width="106%" height="750" style="background: transparent; border: 1px solid #ccc;"></iframe> -->


# Program Committee
<div class="small row-two-columns">
<div class="column-half">
<ul>
{% for people in site.data.pc-members2024 limit:11 %}
<li>{{ people | markdownify | remove: '<p>' | remove: '</p>' | strip }} </li>
{% endfor %}
</ul>
</div>
<div class="column-half">
<ul>
{% for people in site.data.pc-members2024 offset:11 %}
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