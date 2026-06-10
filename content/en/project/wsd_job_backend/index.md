---
title: "YeonHire — Job Posting Platform Backend"
tags: ["project"]
date: 2024-12-10
reading_time: false
summary: "Backend for 'YeonHire', a job-posting platform (Flask & MySQL, solo project)"
---

**Overview —** The backend server for 'YeonHire', a web app for searching and applying to job postings.

<div class="proj-highlight">
Designed and built the entire backend solo — from posting <strong>crawling</strong> to <strong>JWT authentication</strong> and <strong>Swagger API docs</strong>.
</div>

- **Context:** Personal project · 2024.12.10 ~ 12.20
- **Team:** Solo project

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">Backend</span>
<span class="tech-badge">Python</span><span class="tech-badge">Flask</span><span class="tech-badge">Flask-SQLAlchemy</span>
<span class="cat">Auth / Docs</span>
<span class="tech-badge">JWT</span><span class="tech-badge">Swagger (OpenAPI)</span>
<span class="cat">Database</span>
<span class="tech-badge">MySQL</span>
</div>

## Details — Problem → Solution → Result

- **Posting data (postings):** Registering postings manually is hard → a **crawler** auto-collects external postings → fresh postings land in the DB as a search base
- **Auth & security (auth):** Personal data like applications/favorites needs protection → implemented **JWT auth** to identify users by token → only authenticated users can access applications/favorites
- **Applications/favorites (apply):** Users couldn't manage their applications/interests → built **REST APIs** for applications & favorites → users manage their history and saved postings at a glance
- **Collaboration (docs):** API specs were hard to grasp externally → auto-documented with **Swagger UI** → frontend/collaborators can check and integrate immediately

## My Role — Solo Project

- Planning: backend structure & API design for YeonHire
- Development: Flask REST APIs (auth·postings·applications·favorites), posting crawler, Swagger docs

## Infra / Data

- Designed the **MySQL** schema and mapped it via **Flask-SQLAlchemy (ORM)**, structuring REST endpoints by resource

[GitHub Repository](https://github.com/juyeon777/WSD-job-backend)
