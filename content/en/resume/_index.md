---
title: 'Resume'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: markdown
    id: resume-hero
    content:
      text: |
        <div class="resume-hero">
          <h1 class="resume-name">Park Ju Yeon</h1>
          <p class="resume-tagline">A developer building real-world systems across backend, data and IoT</p>
          <p class="resume-contact">
            <a href="mailto:okk1829@gmail.com">okk1829@gmail.com</a>
            <span>·</span>
            <a href="https://github.com/juyeon777" target="_blank">github.com/juyeon777</a>
          </p>
          <a href="/WSD_portfolio/uploads/resume.pdf" target="_blank" class="resume-download">📄 Download Résumé (PDF)</a>
        </div>
    design:
      columns: '1'

  - block: markdown
    id: resume-skills
    content:
      text: |
        <h2 class="resume-h2">Skills</h2>
        <div class="tech-badges resume-badges">
        <span class="cat">Languages</span>
        <span class="tech-badge">Python</span><span class="tech-badge">Java</span><span class="tech-badge">C</span><span class="tech-badge">C++</span><span class="tech-badge">JavaScript</span>
        <span class="cat">Backend &amp; Data</span>
        <span class="tech-badge">Flask</span><span class="tech-badge">MySQL</span><span class="tech-badge">PostgreSQL / TimescaleDB</span><span class="tech-badge">JWT</span><span class="tech-badge">Swagger</span><span class="tech-badge">ML (RandomForest·XGBoost·LightGBM)</span>
        <span class="cat">Frontend</span>
        <span class="tech-badge">Vue</span><span class="tech-badge">React</span><span class="tech-badge">HTML / CSS</span>
        <span class="cat">IoT &amp; Infra</span>
        <span class="tech-badge">Arduino</span><span class="tech-badge">Raspberry Pi</span><span class="tech-badge">MQTT / RabbitMQ</span><span class="tech-badge">Docker</span><span class="tech-badge">AWS</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
        </div>
    design:
      columns: '1'

  - block: markdown
    id: resume-projects
    content:
      text: |
        <h2 class="resume-h2">Selected Projects</h2>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">Seed Propagation Room Digital Twin</span>
            <span class="resume-proj-date">2026.03–06</span>
          </div>
          <p class="resume-proj-meta">Capstone · 5-person team (IoT part)</p>
          <ul>
            <li>IoT digital twin using <strong>real devices and real data</strong> from a demonstration farm, via industry collaboration with Head-IT Inc.</li>
            <li>Designed and validated an end-to-end pipeline "Arduino → Raspberry Pi → MQTT → RabbitMQ → backend → TimescaleDB", collecting 6 sensor types in real time</li>
            <li>Removed location constraints by switching to hotspot communication, implemented freshness-based anomaly detection → deployed on Docker · Azure VM</li>
          </ul>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">City-Bus Passenger Prediction Research</span>
            <span class="resume-proj-date">2024.02–2025.08</span>
          </div>
          <p class="resume-proj-meta">KCI paper (2nd author)</p>
          <ul>
            <li>Predicted passenger demand <strong>without alighting data</strong> from transit-card big data and re-boarding info (RF·XGBoost·LightGBM compared → LightGBM optimal)</li>
            <li>Collected one month of on-board re-boarding data for route 165, joined collaboration meetings, reviewed prior research</li>
            <li>Published in the Journal of KSCI (JKSCI) Vol.30 No.8 (2025.08)</li>
          </ul>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">YeonHire — Job-Posting Platform Backend</span>
            <span class="resume-proj-date">2024.12</span>
          </div>
          <p class="resume-proj-meta">Personal project</p>
          <ul>
            <li>Built a Flask REST API with job-posting crawling, JWT auth and apply/bookmark features; designed the MySQL schema</li>
            <li>Documented the API with Swagger for a collaboration-ready form</li>
          </ul>
        </div>
    design:
      columns: '1'

  - block: experience
    id: education
    content:
      username: admin
    design:
      # Hugo date format
      date_format: 'January 2006'
      # Education or Experience section first?
      is_education_first: false

  - block: markdown
    id: resume-certs
    content:
      text: |
        <h2 class="resume-h2">Certifications &amp; Achievements</h2>
        <ul class="resume-certs">
          <li><strong>KCI paper</strong> — Journal of KSCI (2nd author, 2025.08)</li>
          <li><strong>Engineer Information Processing</strong> — written exam passed (2025.08) · preparing practical exam</li>
          <li>Linux Master Level 2 · Korean History Proficiency Test Advanced Level 3 (2024.10)</li>
          <li>TOEIC Speaking IM3 (2024.11)</li>
        </ul>
    design:
      columns: '1'

  - block: languages
    content:
      title: Languages
      username: admin
---
