---
title: "Github Pages로 개인 페이지 소개 (포폴) 웹사이트 만들기"
tags: ["project"]
date: 2024-09-19
reading_time: false
summary: "OSS 과목에서 만든 개인 포트폴리오 웹사이트 (현재 사이트로 리뉴얼)"
---

**서비스 개요 —** 개인 포트폴리오를 소개하는 웹사이트를 직접 만들어 GitHub Pages로 배포한 프로젝트입니다.

<div class="proj-highlight">
메뉴 탭조차 없는 <strong>빈 템플릿을 처음부터 구현</strong>해야 했고 기간 내 커밋 제한으로 아쉽게 마감했지만, 이후 <strong>현재의 포트폴리오 사이트로 리뉴얼</strong>까지 이어간 점이 특징입니다.
</div>

- **진행 환경:** OSS(오픈소스SW) 수업 · 개인 프로젝트 · 2024.09.19 ~ 10.06
- **참여 인력:** 개인 프로젝트 (단독 진행)

<!--more-->

## 기술 스택

<div class="tech-badges">
<span class="cat">Frontend</span>
<span class="tech-badge">HTML</span><span class="tech-badge">CSS</span><span class="tech-badge">JavaScript</span>
<span class="cat">빌드 / 배포</span>
<span class="tech-badge">Hugo</span><span class="tech-badge">Git</span><span class="tech-badge">GitHub Pages</span>
</div>

## 프로젝트 상세 — 문제 → 해결 → 결과

- **빈 템플릿 (구현):** 선택한 템플릿에 메뉴 탭·기본 코드조차 없어 그대로 쓸 수 없음 → HTML·CSS·JS로 **레이아웃과 메뉴를 처음부터 직접 구현** → 정적 페이지의 기본 구조를 스스로 만들어봄
- **기간 제약 (회고):** 커밋 제한 시점에 템플릿 교체가 불가능해 미완성으로 마감 → 한계를 **회고로 남기고** 재도전 목표를 설정 → "끝까지 완성한다"는 기준이 생긴 계기가 됨
- **리뉴얼 (배포):** 미완성 결과물을 개선하고 싶음 → 새로운 구조(Hugo Blox)로 **현재 포트폴리오 사이트를 다시 구축**하고 배포 → 지금 보고 계신 사이트로 완성

## 담당 역할 — 개인 프로젝트

- 기획: 개인 포트폴리오 웹사이트 기획
- 개발: 템플릿 기반으로 직접 구현 (이후 현재 사이트로 리뉴얼)
- 배포: GitHub Pages

## 인프라 / 배포

- **GitHub Pages**로 정적 사이트를 배포하고, 리뉴얼 버전은 **GitHub Actions 자동 빌드·배포** 파이프라인으로 운영

[배포 사이트](https://juyeon777.github.io/WSD_portfolio/)
[GitHub 저장소](https://github.com/juyeon777/WSD_portfolio)
