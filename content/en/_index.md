---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: biography
    content:
      username: admin
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download Résumé
        url: uploads/resume.pdf
    design:
      banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        filename: abstract-textured-background.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    id: work-style
    content:
      title: Personality & Work Style
      text: |
        <div class="ws-quote">
        <p class="ws-quote-main">Shoot for the moon. Even if you miss, you'll land among the stars.</p>
        <p class="ws-quote-sub">Yesterday is gone, tomorrow is far, today is still unknown.</p>
        </div>
        <p class="ws-lead">I aim high, but I prove it by polishing the result to the end. I first set clear evaluation criteria and judge against them, pinpoint the specific problems in the output, and raise the quality through iterative improvement. I don't stop at planning — I set up version control and a structured working environment to actually execute.</p>
        <div class="ws-label">Strengths</div>
        <div class="ws-grid">
        <div class="ws-card">I break evaluation criteria down and use them as decision-making standards<span class="ws-card-note">judging by criteria, not vague impressions</span></div>
        <div class="ws-card">I pinpoint problems in the output as concrete action items and improve iteratively</div>
        <div class="ws-card">I distinguish what I want to do from what can realistically be finished within the deadline</div>
        <div class="ws-card">I prioritize and allocate limited time based on patterns and evidence</div>
        <div class="ws-card">I don't stop at planning — I build the working environment (Git, modularization) and execute</div>
        <div class="ws-card">I set concrete goals and design my preparation around them</div>
        </div>
        <div class="ws-label">Growth Points</div>
        <ul class="ws-growth">
        <li>Because my quality bar is high, finding the initial direction can take a while, so I set a "decision deadline" and choose within it</li>
        <li>Since I prefer improving quality through rework, in collaboration I first try to agree on "what level is good enough"</li>
        <li>My feedback can get terse, so I consciously add the background context along with the conclusion</li>
        </ul>
    design:
      columns: '1'
---
