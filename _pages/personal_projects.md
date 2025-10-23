---
layout: archive
title: "Personal Projects"
author_profile: true
redirect_from:
  - /personal_projects.html
---


{% include base_path %}


## Company rebrand/pivot detector
During my time at [Beauhurst](https://www.beauhurst.com/), one of my regular tasks was to compare company blurbs, which are short self-descriptions scraped from websites, across different time periods. The goal was to identify cases where a company had rebranded, meaning a significant change in its public image, or pivoted, meaning a change in its products or services. This process was entirely manual and very time-consuming, so I took the initiative to automate it. I developed a natural language processing model using [NLTK](https://www.nltk.org/) to automatically detect when such changes occurred. The model normalises and embeds the text of each blurb into a semantic space where similarity can be quantified, allowing potential rebrands or pivots to be flagged for review. This saved a substantial amount of analyst time and with the concept later incorporated into other workflows within the company.

[code](https://github.com/dominicjbroadbent/pr_detector)

<figure>
  <img src="/images/pivot.png" 
       alt="Text before an after pivot in services." 
       style="max-width:100%; height:auto;">
  <figcaption>
    <em>Example output from the blurb comparison model, showing two versions of a company description with a low similarity score (0.11), indicating a likely rebrand or shift in focus.</em>
  </figcaption>
</figure>
