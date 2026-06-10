---
title: "Car System — Software Engineering Team Project"
tags: ["project"]
date: 2024-12-05
reading_time: false
summary: "A car system built with SRS & TDD (software-engineering team project — docs lead)"
---

**Overview —** A team project that models a car system (engine · pedals · gear · doors/locks · trunk) and implements it in Python.

<div class="proj-highlight">
Followed the full software-engineering process step by step — <strong>SRS</strong> → <strong>TDD</strong> → <strong>version control</strong> (Git/Sourcetree) → <strong>code inspection</strong>.
</div>

- **Context:** Software Engineering course · team project · Fall 2024
- **Team:** Team project (divided roles) — I owned the **SRS / implementation report (documentation)**

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">Development</span>
<span class="tech-badge">Python</span><span class="tech-badge">unittest (TDD)</span>
<span class="cat">VCS / Tools</span>
<span class="tech-badge">Git / GitHub</span><span class="tech-badge">Sourcetree</span><span class="tech-badge">PyCharm</span>
</div>

## Details — Problem → Solution → Result

- **Requirements (SRS):** Criteria were vague before coding → wrote an **SRS** to fix features/constraints in writing → gave the whole team a shared basis to build on
- **Safety logic (impl·test):** Wrong inputs could cause system errors → wrote, via TDD, logic where **the engine starts only while the brake is pressed** → guaranteed the safety condition by tests
- **Concurrent input (impl·test):** Command order changes the result → built & validated order-aware handling via TDD → consistent behavior even in edge cases
- **Documentation (report):** Implementation was hard to follow externally → summarized design & test results in a report → secured traceability and an evaluation basis

## My Role — My Part

- **Documentation lead** — wrote the SRS and the implementation report

## Collaboration / Process

- Within a workflow applying **TDD · version control · code inspection** (not just coding), I kept the docs as the team's shared reference

[GitHub Repository](https://github.com/juyeon777/Software_Engineering_2024)
