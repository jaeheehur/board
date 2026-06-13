# Jaehee's Board

GitHub Pages로 호스팅되는 개인 마크다운 게시판입니다.

🔗 **사이트**: [https://jaeheehur.github.io/board/](https://jaeheehur.github.io/board/)

## 기능

- 마크다운으로 글 작성
- 실시간 미리보기 에디터
- GitHub API를 통해 직접 업로드 (별도 서버 불필요)
- 게시판 목록: 제목, 내용 미리보기, 날짜/시간 표시

## 글쓰기 설정

1. [GitHub PAT 발급](https://github.com/settings/tokens/new?scopes=repo&description=Board+Writer) — `repo` 권한 필요
2. 사이트 접속 후 **설정(⚙️)** 버튼 클릭
3. PAT 입력 후 저장
4. **글쓰기** 버튼으로 글 작성 및 업로드

## 구조

```
board/
├── index.html      # 메인 게시판 SPA
├── posts/          # 게시글 마크다운 파일
│   └── YYYY-MM-DD-timestamp-slug.md
└── README.md
```

## 게시글 형식

```markdown
---
title: 제목
date: 2026-06-13T21:00:00.000Z
image: https://example.com/image.jpg  (선택)
---

본문 내용 (마크다운)
```
