---
title: "실시간 날씨 대시보드"
tags: ["project"]
date: 2024-12-20
reading_time: false
summary: "OpenWeatherMap·AWS 기반 실시간 날씨 대시보드"
---

- **진행 기간:** 2024-12-20 ~ 2024-12-23
- OpenWeatherMap API를 사용해 특정 도시(서울·전주)의 실시간 날씨 데이터를 수집·시각화하는 대시보드 애플리케이션입니다. 온도·습도·풍속을 실시간 그래프로 표시하고, 수집한 데이터는 CSV로 저장합니다.
- **기술 스택:** Python, OpenWeatherMap API, AWS (S3, CloudWatch)

**담당 역할 — 개인 프로젝트**

- 기획: 서울·전주 대상 실시간 날씨 모니터링 대시보드 구상
- 개발: OpenWeatherMap API로 날씨 데이터 주기적 수집 → CSV 저장 → 온도·습도·풍속 실시간 그래프 시각화 (Python, 모듈 분리: fetch/visualize/aws)
- 인프라: AWS S3 업로드·CloudWatch 로그 연동, CloudShell에서 실행해 CloudWatch 대시보드로 실시간 시각화

[GitHub 저장소](https://github.com/juyeon777/weather-dashboard)
