# Blog Posts Archive

Voice-Pro 관련 블로그/홍보 게시글의 원본을 보관하는 폴더입니다. 게시 전 초안과 게시 완료본을 모두 이곳에 둡니다.

## 파일 네이밍 규칙

```
YYYY-MM-DD.<topic-slug>.<platform>.<lang>.md
```

| 구성 요소 | 설명 | 예시 |
|---|---|---|
| `YYYY-MM-DD` | 작성일 (파일명 정렬 = 시간순 정렬) | `2026-07-13` |
| `topic-slug` | 주제를 나타내는 영문 kebab-case 슬러그 | `v4.0.0-release` |
| `platform` | 게시 대상 플랫폼 | `naver`, `tistory`, `medium`, `x` |
| `lang` | 언어 코드 — `docs/README.*.md`와 동일한 접미사 사용 | `kor`, `eng`, `jpn` |

예: `2026-07-13.v4.0.0-release.naver.kor.md`

## 파일 헤더

각 게시글 상단에 HTML 주석으로 메타데이터를 기록합니다 (README 파일들과 동일한 방식):

```html
<!--
    title: 게시글 제목
    platform: Naver Blog
    language: Korean
    date: YYYY-MM-DD
    status: draft | published
    published-url: (게시 후 URL 기입)
    related-release: (관련 GitHub 릴리스 URL)
-->
```

## 본문 형식

- 네이버 블로그 등 마크다운을 렌더링하지 않는 플랫폼용 글은 **붙여넣기 즉시 사용 가능한 일반 텍스트**로 작성합니다 (`**굵게**` 같은 마크다운 문법 사용 금지).
- 마크다운을 지원하는 플랫폼(Medium, GitHub 등)용 글은 마크다운으로 작성해도 됩니다.
- 게시 후에는 헤더의 `status`를 `published`로 바꾸고 `published-url`을 기입합니다.
