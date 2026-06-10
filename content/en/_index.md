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
        ### "Shoot for the moon. Even if you miss, you'll land among the stars."

        *"Yesterday is gone, tomorrow is far, today is still unknown."*

        I aim high, but I prove it by polishing the result to the end. I first set clear evaluation criteria and judge against them, pinpoint the specific problems in the output, and raise the quality through iterative improvement. I don't stop at planning — I set up version control and a structured working environment to actually execute.

        **Strengths**

        - I break evaluation criteria down and use them as decision-making standards (judging by criteria, not vague impressions)
        - I pinpoint problems in the output as concrete action items and improve iteratively
        - I distinguish what I want to do from what can realistically be finished within the deadline
        - I prioritize and allocate limited time based on patterns and evidence
        - I don't stop at planning — I build the working environment (Git, modularization, etc.) and execute
        - I set concrete goals and design my preparation around them

        **Growth Points**

        - Because my quality bar is high, finding the initial direction can take a while, so I set a "decision deadline" and choose within it
        - Since I prefer improving quality through rework, in collaboration I first try to agree on "what level is good enough"
        - My feedback can get terse, so I consciously add the background context along with the conclusion
    design:
      columns: '1'
---
