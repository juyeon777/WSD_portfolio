---
title: "Real-time Weather Dashboard"
tags: ["project"]
date: 2024-12-20
reading_time: false
summary: "A real-time weather dashboard powered by OpenWeatherMap & AWS"
---

- **period:** 2024-12-20 ~ 2024-12-23
- A dashboard application that collects and visualizes real-time weather data for specific cities (Seoul, Jeonju) using the OpenWeatherMap API. It displays temperature, humidity, and wind speed on real-time graphs and saves the collected data as CSV.
- **Tech Stack:** Python, OpenWeatherMap API, AWS (S3, CloudWatch)

**My Role — Personal Project**

- Planning: Designed a real-time weather monitoring dashboard for Seoul and Jeonju
- Development: Periodically fetched weather data via the OpenWeatherMap API → saved to CSV → visualized temperature/humidity/wind on real-time graphs (Python; modular: fetch/visualize/aws)
- Infrastructure: Integrated AWS S3 upload & CloudWatch logging; ran on CloudShell to visualize in real time on a CloudWatch dashboard

[GitHub Repository](https://github.com/juyeon777/weather-dashboard)
