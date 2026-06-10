---
title: "YeonHire — 채용 공고 플랫폼 백엔드"
tags: ["project"]
date: 2024-12-10
reading_time: false
summary: "Flask·MySQL로 만든 채용 공고 플랫폼 'YeonHire' 백엔드 (개인 프로젝트)"
---

**서비스 개요 —** 채용 공고를 검색·지원할 수 있는 웹 애플리케이션 'YeonHire'의 백엔드 서버입니다.

공고 **크롤링**부터 **JWT 인증**, **Swagger API 문서화**까지 백엔드 전 과정을 단독으로 설계·구현한 점이 특징입니다.

- **진행 환경:** 개인 프로젝트 · 2024.12.10 ~ 12.20
- **참여 인력:** 개인 프로젝트 (단독 진행)

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">Backend</span>
<span class="tech-badge">Python</span><span class="tech-badge">Flask</span><span class="tech-badge">Flask-SQLAlchemy</span>
<span class="cat">Auth / Docs</span>
<span class="tech-badge">JWT</span><span class="tech-badge">Swagger (OpenAPI)</span>
<span class="cat">Database</span>
<span class="tech-badge">MySQL</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **공고 데이터 확보 (공고 도메인):** 채용 공고를 일일이 등록·관리하기 어려움 → 공고 **크롤러**로 외부 채용 공고를 자동 수집 → 최신 공고를 DB에 적재해 검색의 기반을 마련
- **인증·보안 (인증 도메인):** 지원 내역·즐겨찾기 같은 개인 데이터 보호 필요 → **JWT 기반 인증**을 구현해 토큰으로 사용자를 식별 → 인증된 사용자만 지원·즐겨찾기에 접근하도록 보호
- **지원/즐겨찾기 (지원 도메인):** 사용자가 지원 현황·관심 공고를 관리할 수 없음 → 지원·즐겨찾기 **REST API** 구현 → 자신의 지원 내역과 관심 공고를 한눈에 관리
- **협업성 (문서화):** API 명세를 외부가 파악하기 어려움 → **Swagger UI**로 자동 문서화 → 프론트엔드·협업자가 바로 확인·연동할 수 있는 형태로 정비

## 담당 역할 — 개인 프로젝트

- 기획: 채용 공고 플랫폼(YeonHire) 백엔드 구조·API 설계
- 개발: Flask 기반 REST API(인증·공고·지원·즐겨찾기) 구현, 공고 크롤러 개발, Swagger 문서화

## 인프라 / 데이터

- **MySQL** 스키마를 설계하고 **Flask-SQLAlchemy(ORM)** 로 매핑, 자원 단위로 REST 엔드포인트를 구조화

[GitHub 저장소](https://github.com/juyeon777/WSD-job-backend)
