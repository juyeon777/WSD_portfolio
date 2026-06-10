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
        <div class="ws-chips">
        <span class="ws-chip">Break criteria down → adopt as decision standards</span>
        <span class="ws-chip">Pinpoint problems as concrete actions → iterate</span>
        <span class="ws-chip">Separate "want to do" vs "doable by deadline"</span>
        <span class="ws-chip">Prioritize & allocate time by patterns/evidence</span>
        <span class="ws-chip">Beyond planning → build the workflow (Git, modules)</span>
        <span class="ws-chip">Concrete goals → tailored preparation</span>
        </div>
        <div class="ws-label">Growth Points</div>
        <ul class="ws-growth">
        <li>A high quality bar can slow early exploration → I set a "decision deadline" and choose within it</li>
        <li>I prefer rework → I first agree on "what's good enough" in collaboration</li>
        <li>My feedback can get terse → I add background context to the conclusion</li>
        </ul>
    design:
      columns: '1'
  - block: markdown
    id: featured-projects
    content:
      title: Featured Projects
      text: |
        <div class="fp-grid">
        <a class="fp-card" href="project/seedlab_digitaltwin/"><img src="project/seedlab_digitaltwin/featured.png" alt="Seed Lab Digital Twin" loading="lazy"><div class="fp-body"><p class="fp-title">Seed Lab Digital Twin</p><p class="fp-desc">A web digital twin that monitors a seed propagation room in real time via IoT sensors (capstone, 5-person team)</p></div></a>
        <a class="fp-card" href="project/project2_lab/"><img src="project/project2_lab/featured.png" alt="City Bus Passenger Prediction" loading="lazy"><div class="fp-body"><p class="fp-title">City-Bus Passenger Prediction</p><p class="fp-desc">ML-based passenger prediction on transit-card big data — published in a KCI paper (2nd author)</p></div></a>
        <a class="fp-card" href="project/sw_engineering_car/"><img src="project/sw_engineering_car/featured.png" alt="Car System" loading="lazy"><div class="fp-body"><p class="fp-title">Car System (SW Engineering)</p><p class="fp-desc">A car-system team project built with an SRS and TDD</p></div></a>
        </div>
        <div class="fp-more"><a href="project/">View all projects →</a></div>
    design:
      columns: '1'
---
