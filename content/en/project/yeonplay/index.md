---
title: "YeonPlay — Front-End Demo Site"
tags: ["project"]
date: 2025-07-15
reading_time: false
summary: "A Vue front-end demo site for browsing movie info (incl. renewal)"
---

**Overview —** A Vue front-end demo site for browsing movie info (now-playing · trending · by-genre · favorites).

<div class="proj-highlight">
Built the screens/features actively using GPT, then <strong>renewed the structure in a separate repository</strong>.
</div>

- **Context:** Personal project · 2024.11 ~ 2025.11
- **Team:** Solo project

<!--more-->

## Tech Stack

<div class="tech-badges">
<span class="cat">Frontend</span>
<span class="tech-badge">Vue</span><span class="tech-badge">JavaScript</span><span class="tech-badge">HTML</span><span class="tech-badge">CSS</span>
<span class="cat">Deploy</span>
<span class="tech-badge">Netlify</span>
</div>

## Details — Problem → Solution → Result

- **Content browsing (UI):** Needed one place to browse movie info → built **category screens** (now-playing · trending · by-genre · favorites) in Vue → users explore movies by category
- **Component structure (frontend):** Code grew complex as screens increased → split screens/features into **components** → organized into a reusable structure
- **Renewal (improvement):** Felt structural limits in the first build → **redesigned and renewed** in a separate repo → improved into a more maintainable form

## My Role — Solo Project

- Planning: planned the movie-browsing demo site
- Development: built screens/features in Vue (using GPT)
- Renewal: improved the structure in a separate repo

## Data / Integration

- Bound the movie data the screens need as **external data into components**, separating the presentation layer from the data

[Live Site](https://yeonplay.netlify.app/)
[GitHub Repository](https://github.com/juyeon777/YeonPlay)
