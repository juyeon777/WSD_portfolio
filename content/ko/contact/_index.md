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
        <h1 class="page-title text-4xl tracking-tight">연락처</h1>
        <p class="page-subtitle">궁금한 점이나 협업 제안이 있다면 편하게 연락 주세요.</p>
    design:
      columns: '1'
  - block: contact
    id: contact
    content:
      title: 연락 정보
      email: okk1829@gmail.com
      #phone: +82 010-2542-2638
      address:
        street: 전북대학교 공과대학 7호관
        city: 전주시
        region: 전라북도
        postcode: '54896'
        country: 대한민국
        country_code: KO
      coordinates:
        latitude: "35.846038"
        longitude: "127.134457"
      directions:
      # Automatically link email and phone or display as text?
      autolink: true
      # 연락 폼 (실제 전송은 Formspree 연동 필요)
      form:
        provider: formspree
        formspree:
          id: xpqelbzj
    design:
    # view: text
      columns: 3
---
