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
        <div class="ws-chips">
        <span class="ws-chip">평가 기준 분해 → 의사결정 기준 채택</span>
        <span class="ws-chip">문제를 행동 단위로 짚어 반복 개선</span>
        <span class="ws-chip">하고 싶은 것 vs 기한 내 가능한 것 구분</span>
        <span class="ws-chip">패턴·근거로 우선순위화해 시간 배분</span>
        <span class="ws-chip">기획에 그치지 않고 작업 환경(Git·모듈화)까지 구축</span>
        <span class="ws-chip">구체적 목표 → 맞춤 준비 설계</span>
        </div>
        <div class="ws-label">성장 포인트</div>
        <ul class="ws-growth">
        <li>완성도 기준이 높아 초기 탐색이 길어질 때 → '결정 마감선'을 정해 선택</li>
        <li>재작업을 선호 → 협업 시 '충분한 선'을 먼저 합의</li>
        <li>피드백이 간결해질 때 → 결론에 배경 맥락을 덧붙임</li>
        </ul>
    design:
      columns: '1'
  - block: markdown
    id: featured-projects
    content:
      title: 대표 프로젝트
      text: |
        <div class="fp-grid">
        <a class="fp-card" href="project/seedlab_digitaltwin/"><img src="project/seedlab_digitaltwin/featured.png" alt="종자 증식실 디지털 트윈" loading="lazy"><div class="fp-body"><p class="fp-title">종자 증식실 디지털 트윈</p><p class="fp-desc">IoT 센서로 종자 증식실을 실시간 모니터링·시각화하는 웹 디지털 트윈 (캡스톤·5인 팀)</p></div></a>
        <a class="fp-card" href="project/project2_lab/"><img src="project/project2_lab/featured.png" alt="시내버스 승객 예측" loading="lazy"><div class="fp-body"><p class="fp-title">시내버스 승객 예측</p><p class="fp-desc">교통카드 빅데이터·머신러닝 기반 승객 예측 — KCI 논문 게재 (제2저자)</p></div></a>
        <a class="fp-card" href="project/sw_engineering_car/"><img src="project/sw_engineering_car/featured.png" alt="자동차 시스템" loading="lazy"><div class="fp-body"><p class="fp-title">자동차 시스템 (SW공학)</p><p class="fp-desc">SRS 작성·TDD 기반으로 구현한 자동차 시스템 팀 프로젝트</p></div></a>
        </div>
        <div class="fp-more"><a href="project/">전체 프로젝트 보기 →</a></div>
    design:
      columns: '1'
---
