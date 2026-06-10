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
    id: featured-projects
    content:
      title: Featured Projects
      text: |
        <div class="fp-carousel-wrap">
        <div class="fp-carousel">
        <a class="fp-card" href="project/seedlab_digitaltwin/"><img src="project/seedlab_digitaltwin/thumb.jpg" alt="Seed Lab Digital Twin" loading="lazy"><span class="fp-tag">Capstone · IoT</span><div class="fp-overlay"><p class="fp-title">Seed Lab Digital Twin</p><p class="fp-desc">A web digital twin monitoring a seed room in real time via IoT</p></div></a>
        <a class="fp-card" href="project/project2_lab/"><img src="project/project2_lab/thumb.jpg" alt="City Bus Passenger Prediction" loading="lazy"><span class="fp-tag">Paper · ML</span><div class="fp-overlay"><p class="fp-title">City-Bus Passenger Prediction</p><p class="fp-desc">ML-based passenger prediction on transit-card big data (KCI paper)</p></div></a>
        <a class="fp-card" href="project/sw_engineering_car/"><img src="project/sw_engineering_car/thumb.jpg" alt="Car System" loading="lazy"><span class="fp-tag">SW Eng.</span><div class="fp-overlay"><p class="fp-title">Car System</p><p class="fp-desc">A car-system team project built with an SRS and TDD</p></div></a>
        </div>
        <button class="fp-nav fp-prev" aria-label="Previous">❮</button>
        <button class="fp-nav fp-next" aria-label="Next">❯</button>
        </div>
        <div class="fp-dots"><button class="fp-dot active" aria-label="1"></button><button class="fp-dot" aria-label="2"></button><button class="fp-dot" aria-label="3"></button></div>
        <div class="fp-more"><a href="project/">View all projects →</a></div>
    design:
      columns: '1'
  - block: markdown
    id: work-style
    content:
      title: Personality & Work Style
      text: |
        <div class="ws-quote">
        <p class="ws-quote-main">Shoot for the moon. Even if you miss, you'll land among the stars.</p>
        <p class="ws-quote-sub">Yesterday is gone, tomorrow is far, today is still unknown.</p>
        </div>
        <p class="ws-lead">I aim high, but I prove it — setting clear criteria and polishing the result to the end. I don't stop at planning; I take it all the way to execution.</p>
        <div class="ws-label">Strengths</div>
        <div class="ws-chips">
        <span class="ws-chip">Break criteria down → adopt as decision standards</span>
        <span class="ws-chip">Pinpoint problems as concrete actions → iterate</span>
        <span class="ws-chip">Prioritize & allocate time by patterns/evidence</span>
        <span class="ws-chip">Beyond planning → build the workflow (Git, modules)</span>
        </div>
    design:
      columns: '1'
---
