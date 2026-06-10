---
title: "종자 증식실 디지털 트윈 시스템"
tags: ["project"]
date: 2026-03-23
reading_time: false
summary: "IoT 센서로 종자 증식실 환경을 실시간 수집·시각화하는 웹 디지털 트윈 (캡스톤·5인 팀, IoT 파트 담당)"
---

[GitHub 저장소](https://github.com/capstone-SeedLabSystem/SeedLabDigitalTwin_System)

- **진행 기간:** 2026 (전북대학교 캡스톤 디자인, 5인 팀 프로젝트)
- **담당 파트:** IoT · 실시간 모니터링
- 종자 증식실의 생육 환경을 IoT 센서로 실시간 수집·시각화하고 원격 제어하는 웹 디지털 트윈 시스템입니다.

<!--more-->

## 주요 기능 (프로젝트 전체)

- **실시간 환경 모니터링:** 대기 온·습도, 토양 온·습도, 일사량, CO₂ 등 6종 센서 데이터를 실시간 수집·표시
- **3D 디지털 트윈:** Three.js 기반으로 증식실·작물·센서·장비 시각화
- **생육 관리:** 로트(Lot) 단위 생육 추적, 영농일지, 작물별 권장환경 추천
- **알림·자동제어:** 임계값 이탈/상태 급변 알림 및 환경 자동제어
- **부가 기능:** 시장가격(KAMIS/aT) 연동, AI 농업 상담 챗봇

## 담당 역할 (본인) — IoT · 실시간 모니터링 파트

**IoT 센서 데이터 파이프라인 구축**

- Arduino UNO R4 WiFi 펌웨어 개발 (6종 센서 데이터 수집)
- 라즈베리파이 게이트웨이(Python, paho-mqtt + systemd) 구현 및 메시지 규약 설계
- 「아두이노 → Pi → MQTT(인증) → Bridge → RabbitMQ → 백엔드 → TimescaleDB」 end-to-end 데이터 파이프라인 설계·검증 (실기기 데이터의 실시간 DB 적재 확인)
- CDS 광저항기 분압회로 설계 및 일사량(W/m²) 환산, CO₂ 온·습도 연관 추정 모델 구현
- 핫스팟 WiFi 이동형 통신 방식 확정(공유기 의존 제거) 및 세팅 매뉴얼 작성
- 라즈베리파이 액추에이터 데몬(MQTT 명령 → GPIO 제어) 운영 배포 및 통합 검증

**실시간 모니터링 웹 기능**

- WebSocket 기반 증식실/로트별 센서 데이터 격리 표시
- 데이터 신선도(staleness) 기반 연결 상태 판정, 센서 최종통신 시각 표시
- 대시보드 상태 표시(정상/주의/미연결) 및 상태 급변(급등·급락) 감지 로직
- 중계기·센서 관리 화면, 모니터링 UI 정리(용어 통일·페이지네이션 등)

**데이터 분석**

- 실측 농가 데이터 분석(t-test/시계열/회귀/상관관계) 및 분석 보고서 작성

## 사용 기술 (본인이 직접 다룬 것)

<style>
.tech-badges{margin:.3rem 0 .5rem;}
.tech-badges .cat{display:block;margin:.7rem 0 .35rem;font-weight:600;font-size:.92em;}
.tech-badge{display:inline-block;padding:3px 11px;margin:3px 6px 3px 0;border-radius:9999px;background:#eef2f7;color:#334155;font-size:.83em;font-weight:500;border:1px solid #e2e8f0;line-height:1.7;}
html.dark .tech-badge{background:#1e293b;color:#cbd5e1;border-color:#334155;}
</style>

<div class="tech-badges">
<span class="cat">IoT / 펌웨어</span>
<span class="tech-badge">Arduino (UNO R4 WiFi)</span><span class="tech-badge">Raspberry Pi</span><span class="tech-badge">Python</span><span class="tech-badge">paho-mqtt</span><span class="tech-badge">gpiozero</span><span class="tech-badge">systemd</span>
<span class="cat">통신 / 메시징</span>
<span class="tech-badge">MQTT (Mosquitto)</span><span class="tech-badge">RabbitMQ</span><span class="tech-badge">WebSocket</span>
<span class="cat">Frontend</span>
<span class="tech-badge">React 18</span><span class="tech-badge">Vite</span><span class="tech-badge">Recharts</span><span class="tech-badge">Axios</span>
<span class="cat">Backend / DB <span style="font-weight:400;font-size:.9em;">(센서·중계기 API 범위)</span></span>
<span class="tech-badge">Spring Boot</span><span class="tech-badge">JPA</span><span class="tech-badge">PostgreSQL</span><span class="tech-badge">TimescaleDB</span>
<span class="cat">데이터 분석</span>
<span class="tech-badge">Python (pandas)</span><span class="tech-badge">통계</span>
<span class="cat">Infra</span>
<span class="tech-badge">Docker Compose</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
</div>
