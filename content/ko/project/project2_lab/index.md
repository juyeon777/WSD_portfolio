---
title: "시내버스의 효율적인 정차를 위한 탑승객 확인 시스템 개발"
tags: ["project"]
date: 2025-08-19
reading_time: false
summary: "산학협력에서 출발한 시내버스 승객 예측 연구 — KCI 논문 게재 (제2저자, 데이터 수집 담당)"
---

**서비스 개요 —** 교통카드 빅데이터로 하차 데이터 없이 시내버스 승객 수요를 예측하는 연구입니다.

<div class="proj-highlight">
2024년 <strong>산학협력 프로젝트</strong>로 시작해, 그 결과를 <strong>한국컴퓨터정보학회논문지(JKSCI) Vol.30 No.8 (2025.08)</strong>에 게재(제2저자)한 점이 특징입니다.
</div>

- **진행 환경:** 산학협력 → 연구 논문 · 2024.02 ~ 2025.08
- **참여 인력:** 지도교수 · 공동연구자(제1저자) · 본인(제2저자) — 본인은 **데이터 수집·자료 조사 담당**

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">머신러닝</span>
<span class="tech-badge">Random Forest</span><span class="tech-badge">XGBoost</span><span class="tech-badge">LightGBM</span>
<span class="cat">데이터 / 도구</span>
<span class="tech-badge">교통카드 빅데이터</span><span class="tech-badge">Python</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **데이터 한계 (수요 예측):** 시내버스는 하차 데이터가 없어 실제 승객 수요 파악이 어려움 → 교통카드 빅데이터와 **재탑승 인원 정보**를 활용해 하차 없이 수요를 추정 → 하차 데이터 부재라는 한계를 우회
- **모델 비교 (방법론):** 어떤 모델이 안정적인지 불확실 → **Random Forest·XGBoost·LightGBM**을 비교 분석 → **LightGBM이 가장 안정적**이라는 결론을 도출
- **연구 성과 (논문):** 결과를 학술적으로 검증·공유할 필요 → 논문으로 정리해 **KCI 등재지에 게재(제2저자)** → 시내버스 정차 효율화에 활용될 근거를 제시

## 담당 역할 — 본인 담당

- 산학협력 단계에서 협력기업(아이테크) 방문 및 회의 참여
- 교통카드 빅데이터 시스템에서 **165번 노선의 차내 재차인원 데이터를 약 한 달간 수집·업데이트**
- 논문 작성을 위한 관련 **선행 연구(논문) 자료 수집**

## 주 업무 외 기여

- 데이터 수집 외에도 산학협력 회의에 참여해 현장 요구를 파악하고, 선행 연구 자료를 모아 논문 작성을 지원

[🔗 KCI에서 논문 보기](https://www.kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003234190)
[📄 논문 PDF 다운로드](paper.pdf)
