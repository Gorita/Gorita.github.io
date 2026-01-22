# 프로젝트 개요: gorita-blog

이 프로젝트는 Jekyll의 'jekyll-theme-chirpy' 테마를 사용하는 개인 기술 블로그입니다.
기술, AI, XR 관련 뉴스 및 분석 글을 공유합니다.

# 기본 규칙
- **언어:** 모든 답변은 한국어로 제공합니다.
- **파일 무시:** `.geminiignore` 폴더 및 그 내부 파일은 무시합니다.
- **Git:** 현재 디렉토리(`gorita-blog`)가 Git 저장소이므로, Git 명령은 이 디렉토리 내에서 실행합니다.

# 프로젝트 구조
- **`_config.yml`**: 사이트 설정 (제목: Gorita, 테마: jekyll-theme-chirpy, 언어: en, 댓글: giscus).
- **`_posts/`**: 게시물 파일 위치. 형식: `YYYY-MM-DD-제목.md`.
- **`_tabs/`**: 상단 탭 페이지 (About, Archives, Categories, Tags).
- **`assets/`**: 정적 리소스 (이미지, CSS 등).
- **`tools/run.sh`**: 로컬 서버 실행 스크립트.

# 워크플로우 가이드

## 1. 로컬 실행
```bash
bash tools/run.sh &
```
서버 주소: `http://127.0.0.1:4000`

## 2. 새 글 작성
`_posts/` 폴더에 `YYYY-MM-DD-영문-제목.md` 파일을 생성하고 아래 Front Matter를 사용합니다.
```yaml
---
title: "글 제목"
date: YYYY-MM-DD HH:MM:SS +0900
categories: [카테고리1, 카테고리2]
tags: [태그1, 태그2]
---
```

## 3. 배포
GitHub Actions를 통해 `main` 브랜치 푸시 시 `https://gorita.github.io`로 자동 배포됩니다.

## 4. 커밋 규칙
- 작업 단위 완료 시 커밋.
- 메시지 형식: `feat: ...`, `fix: ...` 등.
- 커밋 전 항상 사용자 확인 필요.
