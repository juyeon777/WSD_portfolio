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
    id: resume-hero
    content:
      text: |
        <div class="resume-hero">
          <h1 class="resume-name">박주연 <span>Park Ju Yeon</span></h1>
          <p class="resume-tagline">백엔드 · 데이터 · IoT를 아우르며 실제로 쓰이는 시스템을 만드는 개발자</p>
          <div class="resume-actions">
            <a class="resume-btn" href="mailto:okk1829@gmail.com">✉️ okk1829@gmail.com</a>
            <a class="resume-btn" href="https://github.com/juyeon777" target="_blank">🐙 github.com/juyeon777</a>
            <a class="resume-btn resume-btn--primary" href="/WSD_portfolio/uploads/resume.pdf" target="_blank">📄 이력서 PDF 다운로드</a>
          </div>
        </div>
    design:
      columns: '1'

  - block: markdown
    id: resume-skills
    content:
      text: |
        <h2 class="resume-h2">보유 기술</h2>
        <div class="tech-badges resume-badges">
        <span class="cat">Languages</span>
        <span class="tech-badge">Python</span><span class="tech-badge">Java</span><span class="tech-badge">C</span><span class="tech-badge">C++</span><span class="tech-badge">JavaScript</span>
        <span class="cat">Backend &amp; Data</span>
        <span class="tech-badge">Flask</span><span class="tech-badge">MySQL</span><span class="tech-badge">PostgreSQL / TimescaleDB</span><span class="tech-badge">JWT</span><span class="tech-badge">Swagger</span><span class="tech-badge">ML (RandomForest·XGBoost·LightGBM)</span>
        <span class="cat">Frontend</span>
        <span class="tech-badge">Vue</span><span class="tech-badge">React</span><span class="tech-badge">HTML / CSS</span>
        <span class="cat">IoT &amp; Infra</span>
        <span class="tech-badge">Arduino</span><span class="tech-badge">Raspberry Pi</span><span class="tech-badge">MQTT / RabbitMQ</span><span class="tech-badge">Docker</span><span class="tech-badge">AWS</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
        <span class="cat">AI · 바이브코딩</span>
        <span class="tech-badge">Claude Code</span>
        </div>
    design:
      columns: '1'

  - block: markdown
    id: resume-projects
    content:
      text: |
        <h2 class="resume-h2">주요 프로젝트</h2>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">종자 증식실 디지털 트윈 시스템</span>
            <span class="resume-proj-date">2026.03–06</span>
          </div>
          <p class="resume-proj-meta">캡스톤 · 5인 팀 (IoT 파트 담당)</p>
          <ul>
            <li>(주)헤드아이티 산학협력으로 실증 농가의 <strong>실기기·실데이터</strong>를 활용한 IoT 디지털 트윈</li>
            <li>「아두이노 → 라즈베리파이 → MQTT → RabbitMQ → 백엔드 → TimescaleDB」 end-to-end 파이프라인 설계·검증, 6종 센서 실시간 수집</li>
            <li>핫스팟 통신 전환으로 위치 제약 제거, 데이터 신선도 기반 이상 감지 구현 → Docker · Azure VM 배포</li>
          </ul>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">시내버스 승객 예측 연구</span>
            <span class="resume-proj-date">2024.02–2025.08</span>
          </div>
          <p class="resume-proj-meta">KCI 논문 게재 (제2저자)</p>
          <ul>
            <li>교통카드 빅데이터·재탑승 정보로 <strong>하차 데이터 없이</strong> 승객 수요 예측 (RF·XGBoost·LightGBM 비교 → LightGBM 최적)</li>
            <li>165번 노선 1개월 차내 재차인원 데이터 수집, 산학협력 회의 참여, 선행연구 자료 조사</li>
            <li>한국컴퓨터정보학회논문지(JKSCI) Vol.30 No.8 (2025.08) 게재</li>
          </ul>
        </div>
        <div class="resume-proj">
          <div class="resume-proj-head">
            <span class="resume-proj-name">YeonHire — 채용 공고 플랫폼 백엔드</span>
            <span class="resume-proj-date">2024.12</span>
          </div>
          <p class="resume-proj-meta">개인 프로젝트</p>
          <ul>
            <li>Flask REST API로 공고 크롤링 · JWT 인증 · 지원/즐겨찾기 구현, MySQL 스키마 설계</li>
            <li>Swagger로 API 문서화하여 협업 가능한 형태로 정비</li>
          </ul>
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

  - block: markdown
    id: resume-certs
    content:
      text: |
        <h2 class="resume-h2">자격증 &amp; 성과</h2>
        <ul class="resume-certs">
          <li><strong>KCI 논문 게재</strong> — 한국컴퓨터정보학회논문지 (제2저자, 2025.08)</li>
          <li><strong>정보처리기사</strong> 필기 합격 (2025.08) · 실기 준비 중</li>
          <li>리눅스마스터 2급 · 한국사능력검정시험 심화 3급 (2024.10)</li>
          <li>TOEIC Speaking IM3 (2024.11)</li>
        </ul>
    design:
      columns: '1'

  - block: languages
    content:
      title: 언어
      username: admin
---
