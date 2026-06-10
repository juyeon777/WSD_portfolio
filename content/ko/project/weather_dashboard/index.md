---
title: "실시간 날씨 대시보드"
tags: ["project"]
date: 2024-12-20
reading_time: false
summary: "OpenWeatherMap·AWS로 만든 실시간 날씨 대시보드 (개인 프로젝트)"
---

**서비스 개요 —** 특정 도시(서울·전주)의 실시간 날씨를 수집·시각화하는 대시보드 애플리케이션입니다.

데이터 **수집 → 저장 → 시각화 → 클라우드 배포**까지의 흐름을 직접 구성하고 모듈을 분리해 구현한 점이 특징입니다.

- **진행 환경:** 개인 프로젝트 · 2024.12.20 ~ 12.23
- **참여 인력:** 개인 프로젝트 (단독 진행)

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">개발</span>
<span class="tech-badge">Python</span><span class="tech-badge">OpenWeatherMap API</span>
<span class="cat">Cloud / Infra</span>
<span class="tech-badge">AWS S3</span><span class="tech-badge">AWS CloudWatch</span><span class="tech-badge">CloudShell</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **데이터 수집 (수집):** 실시간 날씨를 주기적으로 확보해야 함 → **OpenWeatherMap API**로 서울·전주 날씨를 주기적으로 수집 → 온도·습도·풍속 데이터를 안정적으로 확보
- **저장·시각화 (대시보드):** 수집한 데이터를 보관·확인할 방법 필요 → 데이터를 **CSV로 저장**하고 온도·습도·풍속을 **실시간 그래프**로 시각화 → 도시별 날씨 변화를 한눈에 모니터링
- **모듈화 (구조):** 기능이 섞이면 유지보수가 어려움 → 수집/시각화/AWS 기능을 **모듈로 분리**(fetch·visualize·aws) → 역할이 명확한 구조로 정리

## 담당 역할 — 개인 프로젝트

- 기획: 서울·전주 대상 실시간 날씨 모니터링 대시보드 구상
- 개발: API 수집 → CSV 저장 → 실시간 그래프 시각화 (Python, 모듈 분리)
- 인프라: AWS 연동·운영

## 인프라 / 운영

- **AWS S3**에 데이터를 업로드하고 **CloudWatch** 로그·대시보드와 연동, **CloudShell**에서 실행해 클라우드 환경에서 실시간 시각화

[GitHub 저장소](https://github.com/juyeon777/weather-dashboard)
