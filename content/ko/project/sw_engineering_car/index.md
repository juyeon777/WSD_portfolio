---
title: "자동차 시스템 — 소프트웨어공학 팀 프로젝트"
tags: ["project"]
date: 2024-12-05
reading_time: false
summary: "SRS·TDD로 구현한 자동차 시스템 (소프트웨어공학 팀 프로젝트, 문서·SRS 담당)"
---

**서비스 개요 —** 자동차 시스템(엔진·가속/브레이크 페달·기어·문/잠금장치·트렁크)을 모델링하고 Python으로 구현한 팀 프로젝트입니다.

<div class="proj-highlight">
요구사항 명세서(<strong>SRS</strong>) 작성 → <strong>TDD</strong>(테스트 주도 개발) → <strong>형상관리</strong>(Git/Sourcetree) → <strong>코드 인스펙션</strong>까지 소프트웨어공학 전 과정을 절차대로 밟은 점이 특징입니다.
</div>

- **진행 환경:** 소프트웨어공학 수업 · 팀 프로젝트 · 2024-2학기
- **참여 인력:** 팀 프로젝트(역할 분담) — 본인은 **요구사항 명세서(SRS)·구현 보고서 등 문서화 담당**

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">개발</span>
<span class="tech-badge">Python</span><span class="tech-badge">unittest (TDD)</span>
<span class="cat">형상관리 / 도구</span>
<span class="tech-badge">Git / GitHub</span><span class="tech-badge">Sourcetree</span><span class="tech-badge">PyCharm</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **요구사항 정의 (SRS):** 자동차 동작을 코드로 옮기기 전 기준이 모호함 → **요구사항 명세서(SRS)** 를 작성해 기능·제약을 문서로 확정 → 팀원 전원이 같은 기준으로 구현할 토대를 제공
- **안전 로직 (구현·검증):** 잘못된 조작이 시스템 오류로 이어질 수 있음 → **브레이크가 밟힌 상태에서만 엔진이 켜지는** 안전 로직을 TDD로 작성 → 테스트로 안전 조건을 보장
- **동시 입력 처리 (구현·검증):** 명령의 전후 관계에 따라 결과가 달라짐 → 입력 순서를 고려한 처리 로직을 TDD로 구현·검증 → 예외 상황에서도 일관된 동작을 확보
- **문서화 (보고서):** 구현 내용을 외부가 이해하기 어려움 → 구현 보고서로 설계·테스트 결과를 정리 → 산출물의 추적성과 평가 근거를 확보

## 담당 역할 — 본인 담당

- **보고서·문서화 담당** — 요구사항 명세서(SRS) 작성, 구현 보고서 문서화

## 협업 / 프로세스

- 단순 코딩이 아니라 **TDD·형상관리·코드 인스펙션**을 적용한 협업 흐름에서, 문서가 팀의 공통 기준이 되도록 정리

[GitHub 저장소](https://github.com/juyeon777/Software_Engineering_2024)
