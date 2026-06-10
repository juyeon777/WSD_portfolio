---
title: "YeonPlay — 프론트엔드 데모 사이트"
tags: ["project"]
date: 2025-07-15
reading_time: false
summary: "Vue로 만든 영화 정보 탐색 프론트엔드 데모 사이트 (리뉴얼 포함)"
---

**서비스 개요 —** 영화 정보(현재 상영작·대세·장르별·찜)를 탐색하는 Vue 프론트엔드 데모 사이트입니다.

GPT를 적극 활용해 화면·기능을 구현하고, 이후 **별도 저장소에서 구조를 리뉴얼**한 점이 특징입니다.

- **진행 환경:** 개인 프로젝트 · 2024.11 ~ 2025.11
- **참여 인력:** 개인 프로젝트 (단독 진행)

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">Frontend</span>
<span class="tech-badge">Vue</span><span class="tech-badge">JavaScript</span><span class="tech-badge">HTML</span><span class="tech-badge">CSS</span>
<span class="cat">배포</span>
<span class="tech-badge">Netlify</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **콘텐츠 탐색 (UI):** 영화 정보를 한 곳에서 둘러볼 화면이 필요 → Vue로 현재 상영작·대세·장르별·찜 **카테고리별 화면을 구현** → 사용자가 영화를 분류별로 탐색할 수 있게 함
- **컴포넌트 구조 (프론트엔드):** 화면이 늘면서 코드가 복잡해짐 → 화면·기능을 **컴포넌트 단위로 분리** → 재사용 가능한 구조로 정리
- **리뉴얼 (개선):** 초기 구현의 구조적 한계를 느낌 → 별도 저장소에서 **구조를 다시 설계해 리뉴얼** → 유지보수가 쉬운 형태로 개선

## 담당 역할 — 개인 프로젝트

- 기획: 영화 정보 탐색 데모 사이트 기획
- 개발: Vue로 화면·기능 구현 (GPT 활용)
- 리뉴얼: 별도 저장소에서 구조 개선

## 데이터 / 연동

- 화면에 필요한 영화 데이터를 **외부 데이터 형태로 받아 컴포넌트에 바인딩**하는 구조로 구성해 표현 계층과 데이터를 분리

[배포 사이트](https://yeonplay.netlify.app/)
[GitHub 저장소](https://github.com/juyeon777/YeonPlay)
