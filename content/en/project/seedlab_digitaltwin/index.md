---
title: "Seed Lab Digital Twin System"
tags: ["project"]
date: 2026-03-23
reading_time: false
summary: "A web digital-twin monitoring a seed propagation room via IoT sensors (capstone, 5-person team — IoT part)"
---

- **period:** 2026 (Jeonbuk National University Capstone Design, 5-person team)
- **My part:** IoT · Real-time Monitoring
- A web-based digital twin system that collects, visualizes, and remotely controls the growing environment of a seed propagation room in real time using IoT sensors.

<!--more-->

## Key Features (whole project)

- **Real-time environment monitoring:** real-time collection and display of 6 sensor types — air temp/humidity, soil temp/humidity, solar radiation, CO₂
- **3D digital twin:** visualizes the propagation room, crops, sensors, and equipment with Three.js
- **Growth management:** lot-level growth tracking, farming journal, recommended environment per crop
- **Alerts & auto-control:** threshold-breach / sudden-change alerts and automated environment control
- **Extras:** market price integration (KAMIS/aT), AI agriculture consultation chatbot

## My Role — IoT · Real-time Monitoring part

**Building the IoT sensor data pipeline**

- Developed Arduino UNO R4 WiFi firmware (collecting 6 sensor types)
- Implemented a Raspberry Pi gateway (Python, paho-mqtt + systemd) and designed the message protocol
- Designed and verified the end-to-end pipeline "Arduino → Pi → MQTT (auth) → Bridge → RabbitMQ → Backend → TimescaleDB" (confirmed real-device data is ingested into the DB in real time)
- Designed a CDS photoresistor voltage-divider circuit, converted solar radiation (W/m²), and implemented a CO₂ temperature/humidity correlation estimation model
- Finalized a mobile hotspot WiFi communication method (removing router dependency) and wrote the setup manual
- Deployed and integration-tested a Raspberry Pi actuator daemon (MQTT command → GPIO control)

**Real-time monitoring web features**

- WebSocket-based isolated display of sensor data per propagation room / lot
- Connection-status determination based on data staleness, with last-communication timestamps per sensor
- Dashboard status indicators (normal / caution / disconnected) and sudden-change (spike/drop) detection logic
- Relay & sensor management screens, monitoring UI cleanup (terminology unification, pagination, etc.)

**Data analysis**

- Analyzed real farm data (t-test / time series / regression / correlation) and wrote the analysis report

## Tech Used (hands-on by me)

<style>
.tech-badges{margin:.3rem 0 .5rem;}
.tech-badges .cat{display:block;margin:.7rem 0 .35rem;font-weight:600;font-size:.92em;}
.tech-badge{display:inline-block;padding:3px 11px;margin:3px 6px 3px 0;border-radius:9999px;background:#eef2f7;color:#334155;font-size:.83em;font-weight:500;border:1px solid #e2e8f0;line-height:1.7;}
html.dark .tech-badge{background:#1e293b;color:#cbd5e1;border-color:#334155;}
</style>

<div class="tech-badges">
<span class="cat">IoT / Firmware</span>
<span class="tech-badge">Arduino (UNO R4 WiFi)</span><span class="tech-badge">Raspberry Pi</span><span class="tech-badge">Python</span><span class="tech-badge">paho-mqtt</span><span class="tech-badge">gpiozero</span><span class="tech-badge">systemd</span>
<span class="cat">Communication / Messaging</span>
<span class="tech-badge">MQTT (Mosquitto)</span><span class="tech-badge">RabbitMQ</span><span class="tech-badge">WebSocket</span>
<span class="cat">Frontend</span>
<span class="tech-badge">React 18</span><span class="tech-badge">Vite</span><span class="tech-badge">Recharts</span><span class="tech-badge">Axios</span>
<span class="cat">Backend / DB <span style="font-weight:400;font-size:.9em;">(sensor & relay API scope)</span></span>
<span class="tech-badge">Spring Boot</span><span class="tech-badge">JPA</span><span class="tech-badge">PostgreSQL</span><span class="tech-badge">TimescaleDB</span>
<span class="cat">Data Analysis</span>
<span class="tech-badge">Python (pandas)</span><span class="tech-badge">Statistics</span>
<span class="cat">Infra</span>
<span class="tech-badge">Docker Compose</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
</div>

## Links

- [GitHub Repository](https://github.com/capstone-SeedLabSystem/SeedLabDigitalTwin_System)
