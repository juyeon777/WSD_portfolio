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
          <div class="resume-actions">
            <a class="resume-btn" href="mailto:okk1829@gmail.com">✉️ okk1829@gmail.com</a>
            <a class="resume-btn" href="https://github.com/juyeon777" target="_blank">🐙 github.com/juyeon777</a>
            <a class="resume-btn resume-btn--primary" href="/WSD_portfolio/uploads/resume.pdf" target="_blank">📄 Download Résumé (PDF)</a>
          </div>
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
        <span class="cat">AI · Vibe Coding</span>
        <span class="tech-badge">Claude Code</span>
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
          <p class="resume-proj-line">Designed and validated the end-to-end IoT pipeline (Arduino→Raspberry Pi→MQTT→RabbitMQ→TimescaleDB) and handled real-time collection of 6 sensors and deployment.</p>
          <a class="resume-proj-btn" href="/WSD_portfolio/en/project/seedlab_digitaltwin/">Read more →</a>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">City-Bus Passenger Prediction Research</span>
            <span class="resume-proj-date">2024.02–2025.08</span>
          </div>
          <p class="resume-proj-meta">KCI paper (2nd author)</p>
          <p class="resume-proj-line">Research predicting passenger demand without alighting data from transit-card big data; I handled data collection and prior-research review. (LightGBM optimal · KCI-indexed)</p>
          <a class="resume-proj-btn" href="/WSD_portfolio/en/project/project2_lab/">Read more →</a>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">Car System — Software Engineering Team Project</span>
            <span class="resume-proj-date">2024.12</span>
          </div>
          <p class="resume-proj-meta">Software Engineering · team project</p>
          <p class="resume-proj-line">A team project following the full SE process (SRS→TDD→version control→code inspection); I owned the SRS and documentation.</p>
          <a class="resume-proj-btn" href="/WSD_portfolio/en/project/sw_engineering_car/">Read more →</a>
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
