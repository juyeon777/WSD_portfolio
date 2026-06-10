---
title: "종자 증식실 디지털 트윈 시스템"
tags: ["project"]
date: 2026-06-05
reading_time: false
summary: "종자 증식실 환경을 IoT로 실시간 수집·시각화하고 원격 제어하는 웹 디지털 트윈 (캡스톤·5인 팀, IoT 파트 담당)"
---

**서비스 개요 —** 종자 증식실의 생육 환경을 IoT 센서로 실시간 수집·시각화하고 원격 제어하는 웹 디지털 트윈 서비스입니다.

- **진행 환경:** 전북대학교 **캡스톤 디자인** · 5인 팀 · 2026.03.11 ~ 06.05
- **🔑 핵심 포인트:** **(주)헤드아이티 산학협력** 프로젝트로, 시뮬레이션이 아닌 **실증 농가의 실기기·실데이터**로 end-to-end 검증까지 마친 점
- **참여 인력:** 5인 팀(백엔드 · 프론트엔드 · IoT 분담) — 본인은 **IoT·실시간 모니터링 파트를 단독 담당**

<!--more-->

## 기술 스택

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
<span class="tech-badge">Python (pandas)</span><span class="tech-badge">통계 (t-test·회귀)</span>
<span class="cat">Infra</span>
<span class="tech-badge">Docker Compose</span><span class="tech-badge">Azure VM</span><span class="tech-badge">Git</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **통신 안정화 (실시간 수집 인프라):** 공유기 의존 통신이라 증식실을 옮기면 센서 연결이 끊기는 문제 → **핫스팟 WiFi 이동형 통신**으로 전환해 공유기 의존을 제거하고 세팅 매뉴얼까지 작성 → 위치에 구애받지 않는 **안정적 데이터 수집**을 확보해, 현장 설치 자유도가 올라감
- **데이터 파이프라인 (센서 → DB):** 실기기 센서값이 DB까지 신뢰성 있게 적재되는지 미검증 → 「아두이노 → 라즈베리파이 → MQTT(인증) → Bridge → RabbitMQ → 백엔드 → TimescaleDB」 **end-to-end 파이프라인을 설계·검증** → 실기기 데이터의 **실시간 DB 적재를 입증**, 이후 모든 모니터링 기능의 토대가 됨
- **이상 감지 (모니터링 UI):** 센서 미연결·급변을 사용자가 알아채기 어려움 → 데이터 **신선도(staleness) 기반 연결 상태 판정** + 급등·급락 감지 + 대시보드 상태 표시(정상/주의/미연결) → 농가가 이상 상황을 **즉시 인지**, 생육 환경 이탈로 인한 작물 손실 예방에 기여
- **관리 기능 (Settings):** 운영자가 직접 기기를 다뤄야 함 → **단위코드·중계기·센서 관리 CRUD 화면**을 구현 → 비개발자도 기기를 등록·관리할 수 있게 함

## 인프라 / 운영

- **Docker Compose**로 컨테이너화하고 **Azure VM에 배포**(seedlab.headit.kr), MQTT(인증)·RabbitMQ로 메시지 유실 없는 신뢰성 있는 전송을 구성

## 주 업무 외 기여

- 실측 농가 데이터를 **통계 분석(t-test·시계열·회귀·상관)** 해 보고서로 정리, 통신 세팅 매뉴얼 작성, 라즈베리파이↔백엔드 **통합 검증을 주도**해 팀의 디버깅 시간을 줄임

[배포 사이트](https://seedlab.headit.kr/)
[GitHub 저장소](https://github.com/capstone-SeedLabSystem/SeedLabDigitalTwin_System)
