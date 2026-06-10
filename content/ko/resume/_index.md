---
title: '이력서'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: markdown
    id: resume-download
    content:
      text: |
        <div style="text-align:center;">
          <a href="/WSD_portfolio/uploads/resume.pdf" target="_blank" class="inline-flex items-center px-4 py-2 text-sm font-medium text-gray-900 bg-white border border-gray-200 rounded-lg hover:bg-gray-100 hover:text-primary-700 dark:bg-gray-800 dark:text-gray-400 dark:border-gray-600 dark:hover:text-white dark:hover:bg-gray-700">📄 이력서 PDF 다운로드</a>
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
  - block: skills
    content:
      title: 기술
      username: admin
  - block: languages
    content:
      title: 언어
      username: admin
---
