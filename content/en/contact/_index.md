---
title: Contact
date: 2024-09-30

type: landing


# Page sections
sections:
  - block: markdown
    id: contact-title
    content:
      text: |
        <h1 class="page-title text-4xl tracking-tight">Contact</h1>
        <p class="page-subtitle">Feel free to reach out for questions or collaboration.</p>
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: Contact Information
      email: okk1829@gmail.com
      #phone: +82 010-2542-2638
      address:
        street: Engineering Building 7, Jeonbuk National University
        city: Jeonju
        region: Jeollabuk-do
        postcode: '54896'
        country: South Korea
        country_code: KR
      coordinates:
        latitude: "35.846038"
        longitude: "127.134457"
      directions:
      # Automatically link email and phone or display as text?
      autolink: true
      # Contact form (requires Formspree to actually send)
      form:
        provider: formspree
        formspree:
          id: xpqelbzj
    design:
    # view: text
      columns: 3
---
