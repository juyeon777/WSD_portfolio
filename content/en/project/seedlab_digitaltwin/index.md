---
title: "Seed Lab Digital Twin System"
tags: ["project"]
date: 2026-06-05
reading_time: false
summary: "A web digital-twin monitoring a seed propagation room via IoT sensors (capstone, 5-person team — IoT part)"
---

**Overview —** A web digital twin that collects, visualizes, and remotely controls a seed propagation room's growing environment in real time via IoT sensors.

<div class="proj-highlight">
<strong>Industry partner ·</strong> HEADIT Co., Ltd.<br>
Validated end-to-end with a <strong>real farm's actual devices and live data</strong> — not a simulation
</div>

- **Context:** Jeonbuk National University **Capstone Design** · 5-person team · 2026.03.11 ~ 06.05
- **Team:** 5-person team (backend · frontend · IoT) — I solely owned the **IoT & real-time monitoring** part

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">IoT / Firmware</span>
<span class="tech-badge">Arduino (UNO R4 WiFi)</span><span class="tech-badge">Raspberry Pi</span><span class="tech-badge">Python</span><span class="tech-badge">paho-mqtt</span><span class="tech-badge">gpiozero</span><span class="tech-badge">systemd</span>
<span class="cat">Messaging</span>
<span class="tech-badge">MQTT (Mosquitto)</span><span class="tech-badge">RabbitMQ</span><span class="tech-badge">WebSocket</span>
<span class="cat">Frontend</span>
<span class="tech-badge">React 18</span><span class="tech-badge">Vite</span><span class="tech-badge">Recharts</span><span class="tech-badge">Axios</span>
<span class="cat">Backend / DB</span>
<span class="tech-badge">Spring Boot</span><span class="tech-badge">JPA</span><span class="tech-badge">PostgreSQL</span><span class="tech-badge">TimescaleDB</span>
<span class="cat">Data / Infra</span>
<span class="tech-badge">Python (pandas)</span><span class="tech-badge">Docker Compose</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
</div>

## Details — Problem → Solution → Result

- **Stable communication (real-time pipeline):** Router-dependent comms dropped sensor connections whenever the room moved → switched to **mobile hotspot WiFi** (removing router dependence) with a setup manual → secured **stable collection** regardless of location, improving install flexibility
- **Data pipeline (sensor → DB):** It was unverified whether real-device readings reliably reached the DB → designed & validated an **end-to-end pipeline** (Arduino → Pi → MQTT(auth) → Bridge → RabbitMQ → backend → TimescaleDB) → **proved real-time DB ingestion**, the foundation for every monitoring feature
- **Anomaly detection (monitoring UI):** Users couldn't easily notice disconnects/sudden changes → built **staleness-based connection status** + spike/drop detection + dashboard status (normal/warning/offline) → farms recognize anomalies **immediately**, helping prevent crop loss
- **Management (Settings):** Operators needed to manage devices directly → built **unit-code · gateway · sensor CRUD screens** → even non-developers can register/manage devices

## My Role — IoT & Real-time Monitoring

**IoT sensor data pipeline**

- Developed Arduino UNO R4 WiFi firmware (6 sensor types)
- Built a Raspberry Pi gateway (Python, paho-mqtt + systemd) and designed the message protocol
- Designed & validated the «Arduino → Pi → MQTT(auth) → Bridge → RabbitMQ → backend → TimescaleDB» end-to-end pipeline
- Designed a CDS photoresistor circuit, converted irradiance (W/m²), and built a CO₂ / temp·humidity estimation model
- Deployed & integration-tested the Raspberry Pi actuator daemon (MQTT command → GPIO control)

**Settings screens**

- Built unit-code · gateway · sensor management CRUD screens

**Real-time monitoring web features**

- WebSocket-based per-room/per-lot sensor isolation
- Dashboard status (normal/warning/offline) and spike/drop detection logic
- Monitoring UI cleanup (terminology, alert-history pagination, etc.)

**Data analysis**

- Analyzed real farm data (t-test/time-series/regression/correlation) and wrote an analysis report

## Infra / Operations

- Containerized with **Docker Compose** and deployed to an **Azure VM** (seedlab.headit.kr); configured MQTT(auth) · RabbitMQ for reliable, loss-free messaging

## Beyond My Main Role

- Beyond IoT, I **statistically analyzed** real farm data into a report, wrote the comms setup manual, and **led the Pi↔backend integration testing**, cutting the team's debugging time

[Live Site](https://seedlab.headit.kr/)
[GitHub Repository](https://github.com/capstone-SeedLabSystem/SeedLabDigitalTwin_System)
