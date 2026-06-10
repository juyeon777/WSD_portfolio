---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

# Note: `username` refers to the user's folder name in `content/authors/`

# Page sections
sections:
  - block: biography
    content:
      username: admin
      # Show a call-to-action button under your biography? (optional)
      button:
        text: 이력서 다운로드
        url: uploads/resume.pdf
    design:
      banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        filename: abstract-textured-background.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    id: work-style
    content:
      title: 성격 및 업무 스타일
      text: |
        <div class="ws-quote">
        <p class="ws-quote-main">달을 향해 쏴라, 빗나가도 별이 될 테니</p>
        <p class="ws-quote-sub">어제는 끝났고, 내일은 멀었고, 오늘은 아직 모른다</p>
        </div>
        <p class="ws-lead">높은 목표를 잡되, 결과물을 끝까지 다듬어 증명합니다. 명확한 평가 기준을 먼저 세우고 그에 맞춰 판단하며, 결과물의 문제를 구체적으로 짚어 반복 개선으로 완성도를 끌어올립니다. 기획에 그치지 않고 버전 관리·구조화된 작업 환경까지 세팅해 실제로 실행하는 편입니다.</p>
        <div class="ws-label">강점</div>
        <div class="ws-grid">
        <div class="ws-card">평가 기준 분해 → 의사결정 기준 채택</div>
        <div class="ws-card">문제를 행동 단위로 짚어 반복 개선</div>
        <div class="ws-card">하고 싶은 것 vs 기한 내 가능한 것 구분</div>
        <div class="ws-card">패턴·근거로 우선순위화해 시간 배분</div>
        <div class="ws-card">기획에 그치지 않고 작업 환경(Git·모듈화)까지 구축</div>
        <div class="ws-card">구체적 목표 → 맞춤 준비 설계</div>
        </div>
        <div class="ws-label">성장 포인트</div>
        <ul class="ws-growth">
        <li>완성도 기준이 높아 초기 탐색이 길어질 때 → '결정 마감선'을 정해 선택</li>
        <li>재작업을 선호 → 협업 시 '충분한 선'을 먼저 합의</li>
        <li>피드백이 간결해질 때 → 결론에 배경 맥락을 덧붙임</li>
        </ul>
    design:
      columns: '1'
---
