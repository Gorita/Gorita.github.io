# gorita-blog 프로젝트 요약

이 문서는 `gorita-blog` 프로젝트의 구조와 사용법을 요약합니다.

## 프로젝트 구조

- **`_config.yml`**: 블로그의 주요 설정을 담고 있는 파일입니다. (블로그 제목, 저자, URL 등)
- **`_posts`**: 블로그 게시물이 저장되는 폴더입니다. `YYYY-MM-DD-제목.md` 형식의 마크다운 파일로 게시물을 작성합니다.
- **`_tabs`**: 'About', 'Archives' 등 상단 탭 페이지의 내용을 담고 있습니다.
- **`assets`**: 이미지, CSS, JavaScript 등 블로그의 정적 파일들이 위치합니다. 프로필 이미지 등은 `assets/img/` 폴더에 있습니다.
- **`tools/run.sh`**: 로컬에서 블로그를 실행하기 위한 스크립트입니다.

## 사용 방법

### 로컬에서 블로그 실행하기

1.  터미널에서 `gorita-blog` 폴더로 이동합니다.
    ```bash
    cd gorita-blog
    ```
2.  아래 명령어를 실행하여 로컬 서버를 시작합니다.
    ```bash
    bash tools/run.sh &
    ```
3.  웹 브라우저에서 `http://127.0.0.1:4000` 주소로 접속하여 블로그를 확인할 수 있습니다.

### 새로운 글 작성하기

1.  `_posts` 폴더 안에 `YYYY-MM-DD-글-제목.md` 형식으로 새 마크다운 파일을 생성합니다.
2.  파일 상단에 아래와 같은 형식으로 메타데이터(Front Matter)를 추가합니다.
    ```yaml
    ---
    title: "글 제목"
    date: YYYY-MM-DD HH:MM:SS +0900
    categories: [카테고리1, 카테고리2]
    tags: [태그1, 태그2]
    ---

    여기에 글 내용을 작성합니다.
    ```

### 블로그 배포

이 블로그는 GitHub Actions를 통해 `https://gorita.github.io`에 자동으로 배포되도록 설정되어 있습니다. `main` 브랜치에 변경사항을 푸시하면 잠시 후 사이트에 반영됩니다.

## Google Analytics 설정

Google Analytics ID를 `_config.yml` 파일에 설정하여 블로그 방문자 및 게시물 조회수를 추적하도록 구성되었습니다.
