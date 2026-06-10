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
        url: /WSD_portfolio/uploads/resume.pdf
    design:
      banner:
        # Upload your cover image to the `assets/media/` folder and reference it here
        filename: abstract-textured-background.jpg
      biography:
        # Customize the style of your biography text
        style: 'text-align: justify; font-size: 0.8em;'
  - block: markdown
    id: featured-projects
    content:
      title: 대표 프로젝트
      text: |
        <div class="fp-carousel-wrap">
        <div class="fp-carousel">
        <a class="fp-card" href="project/seedlab_digitaltwin/"><img src="project/seedlab_digitaltwin/thumb.jpg" alt="종자 증식실 디지털 트윈" loading="lazy"><span class="fp-tag">캡스톤 · IoT</span><div class="fp-overlay"><p class="fp-title">종자 증식실 디지털 트윈</p><p class="fp-desc">IoT 센서로 실시간 모니터링하는 웹 디지털 트윈</p></div></a>
        <a class="fp-card" href="project/project2_lab/"><img src="project/project2_lab/thumb.jpg" alt="시내버스 승객 예측" loading="lazy"><span class="fp-tag">논문 · ML</span><div class="fp-overlay"><p class="fp-title">시내버스 승객 예측</p><p class="fp-desc">교통카드 빅데이터·머신러닝 기반 승객 예측 (KCI 논문)</p></div></a>
        <a class="fp-card" href="project/sw_engineering_car/"><img src="project/sw_engineering_car/thumb.jpg" alt="자동차 시스템" loading="lazy"><span class="fp-tag">SW공학</span><div class="fp-overlay"><p class="fp-title">자동차 시스템</p><p class="fp-desc">SRS·TDD로 구현한 자동차 시스템 팀 프로젝트</p></div></a>
        </div>
        <button class="fp-nav fp-prev" aria-label="이전">❮</button>
        <button class="fp-nav fp-next" aria-label="다음">❯</button>
        </div>
        <div class="fp-dots"><button class="fp-dot active" aria-label="1"></button><button class="fp-dot" aria-label="2"></button><button class="fp-dot" aria-label="3"></button></div>
        <div class="fp-more"><a href="project/">전체 프로젝트 보기 →</a></div>
    design:
      columns: '1'
  - block: markdown
    id: work-style
    content:
      title: 성격 및 업무 스타일
      text: |
        <div class="ws-quote">
        <p class="ws-quote-main">달을 향해 쏴라, 빗나가도 별이 될 테니</p>
        <p class="ws-quote-sub">어제는 끝났고, 내일은 멀었고, 오늘은 아직 모른다</p>
        </div>
        <p class="ws-lead">높은 목표를 잡되, 명확한 기준을 세워 결과물을 끝까지 다듬어 증명합니다. 기획에 그치지 않고 실제 실행까지 책임지는 편입니다.</p>
        <div class="ws-label">강점</div>
        <div class="ws-chips">
        <span class="ws-chip">평가 기준 분해 → 의사결정 기준 채택</span>
        <span class="ws-chip">문제를 행동 단위로 짚어 반복 개선</span>
        <span class="ws-chip">패턴·근거로 우선순위화해 시간 배분</span>
        <span class="ws-chip">기획을 넘어 작업 환경(Git·모듈화)까지 구축</span>
        </div>
    design:
      columns: '1'
---
