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
        <div class="ws-card">평가 기준을 분해해 의사결정 기준으로 삼습니다<span class="ws-card-note">막연한 인상이 아니라 기준으로 판단</span></div>
        <div class="ws-card">결과물의 문제를 구체적인 행동 단위로 짚어 반복 개선합니다</div>
        <div class="ws-card">하고 싶은 것과 기한 내 완성 가능한 것을 구분해 현실적으로 판단합니다</div>
        <div class="ws-card">한정된 시간을 패턴·근거로 우선순위화해 배분합니다</div>
        <div class="ws-card">기획에서 끝내지 않고 Git·모듈화 등 작업 환경 구축까지 실행합니다</div>
        <div class="ws-card">구체적 목표를 세우고 거기에 맞춰 준비를 설계합니다</div>
        </div>
        <div class="ws-label">성장 포인트</div>
        <ul class="ws-growth">
        <li>완성도 기준이 높아 초기 방향 탐색이 길어질 때가 있어, '결정 마감선'을 정해두고 그 안에서 선택합니다</li>
        <li>재작업을 통한 품질 향상을 선호해, 협업에서는 '어느 선이 충분한가'를 먼저 합의하려 합니다</li>
        <li>피드백이 간결해질 때가 있어, 결론과 함께 배경 맥락을 덧붙이려 의식합니다</li>
        </ul>
    design:
      columns: '1'
---
