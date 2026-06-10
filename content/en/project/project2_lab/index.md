---
title: "Development of a Passenger Verification System for Efficient Stops of City Buses"
tags: ["project"]
date: 2025-08-19
reading_time: false
summary: "City-bus passenger prediction research that started from an industry-academia collaboration — KCI paper (2nd author, data collection)"
---

**Overview —** Research that predicts city-bus passenger demand from transit-card big data without alighting data.

<div class="proj-highlight">
Started as a <strong>2024 industry-academia collaboration</strong> and published the results in the <strong>Journal of KSCI (JKSCI) Vol.30 No.8 (2025.08)</strong> as 2nd author.
</div>

- **Context:** Industry-academia → research paper · 2024.02 ~ 2025.08
- **Team:** Advising professor · co-researcher (1st author) · me (2nd author) — I owned **data collection & literature research**

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">Machine Learning</span>
<span class="tech-badge">Random Forest</span><span class="tech-badge">XGBoost</span><span class="tech-badge">LightGBM</span>
<span class="cat">Data / Tools</span>
<span class="tech-badge">Transit-card big data</span><span class="tech-badge">Python</span>
</div>

## Details — Problem → Solution → Result

- **Data limit (demand):** City buses have no alighting data, so real demand is hard to gauge → used transit-card big data and **re-boarding counts** to estimate demand without alighting → worked around the missing-data limit
- **Model comparison (method):** It was unclear which model is stable → compared **Random Forest · XGBoost · LightGBM** → concluded that **LightGBM is the most stable**
- **Research outcome (paper):** Results needed academic validation/sharing → wrote it up and **published in a KCI-listed journal (2nd author)** → provided a basis usable for more efficient bus stopping

## My Role — My Part

- Visited the partner company (iTech) and joined meetings during the collaboration phase
- Collected & updated **~1 month of in-vehicle re-boarding data for bus route #165** from the transit-card big-data system
- Gathered **prior-research (paper) materials** for writing

## Beyond My Main Role

- Beyond data collection, I joined collaboration meetings to grasp field needs and gathered prior-research materials to support the writing

[🔗 View paper on KCI](https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003234190)
[📄 Download paper PDF](paper.pdf)
