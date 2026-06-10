---
title: "Real-time Weather Dashboard"
tags: ["project"]
date: 2024-12-20
reading_time: false
summary: "A real-time weather dashboard powered by OpenWeatherMap & AWS (solo project)"
---

**Overview —** A dashboard app that collects and visualizes real-time weather for specific cities (Seoul · Jeonju).

<div class="proj-highlight">
Built the whole flow myself — <strong>collect → store → visualize → cloud deploy</strong> — with separated modules.
</div>

- **Context:** Personal project · 2024.12.20 ~ 12.23
- **Team:** Solo project

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">Development</span>
<span class="tech-badge">Python</span><span class="tech-badge">OpenWeatherMap API</span>
<span class="cat">Cloud / Infra</span>
<span class="tech-badge">AWS S3</span><span class="tech-badge">AWS CloudWatch</span><span class="tech-badge">CloudShell</span>
</div>

## Details — Problem → Solution → Result

- **Collection:** Real-time weather had to be fetched periodically → periodically collected Seoul·Jeonju weather via the **OpenWeatherMap API** → reliably secured temp·humidity·wind data
- **Store · visualize (dashboard):** Collected data needed storage/inspection → **saved to CSV** and visualized temp·humidity·wind as **real-time graphs** → monitor each city's weather at a glance
- **Modularization (structure):** Mixed features hurt maintainability → split collection/visualization/AWS into **modules** (fetch·visualize·aws) → organized a clear-responsibility structure

## My Role — Solo Project

- Planning: a real-time weather-monitoring dashboard for Seoul·Jeonju
- Development: API collection → CSV → real-time graphs (Python, modular)
- Infra: AWS integration & operation

## Infra / Operations

- Uploaded data to **AWS S3**, integrated **CloudWatch** logs/dashboard, and ran it from **CloudShell** for real-time cloud visualization

[GitHub Repository](https://github.com/juyeon777/weather-dashboard)
