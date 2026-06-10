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
        <div class="ws-card">Break criteria down → adopt as decision standards</div>
        <div class="ws-card">Pinpoint problems as concrete actions → iterate</div>
        <div class="ws-card">Separate "want to do" vs "doable by deadline"</div>
        <div class="ws-card">Prioritize & allocate time by patterns/evidence</div>
        <div class="ws-card">Beyond planning → build the workflow (Git, modules)</div>
        <div class="ws-card">Concrete goals → tailored preparation</div>
        </div>
        <div class="ws-label">Growth Points</div>
        <ul class="ws-growth">
        <li>A high quality bar can slow early exploration → I set a "decision deadline" and choose within it</li>
        <li>I prefer rework → I first agree on "what's good enough" in collaboration</li>
        <li>My feedback can get terse → I add background context to the conclusion</li>
        </ul>
    design:
      columns: '1'
---
