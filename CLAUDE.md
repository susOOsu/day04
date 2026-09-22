# susu 포트폴리오

## 목적
디자인 작업물을 소개하는 개인 포트폴리오 사이트.

## 핵심 기능
- 자기소개
- 작업물 목록
- 작업물 상세
- 로그인
- 작업물 등록/수정/삭제

## 현재 상태
아직 위 기능 대부분은 구현 전이며, 정적 페이지와 Supabase 연동을 연습하는 단계다.

- `index.html`, `about.html` — 기본 정적 페이지
- `preview.html` — Supabase `test_todos` 테이블 데이터를 표로 조회하는 연습 페이지 (실제 포트폴리오 기능이 아닌 Supabase 연동 테스트용)
- `style.css` — 전체 페이지 공통 스타일시트 (은은한 코랄 톤)

## 기술 스택 / 컨벤션
- 별도 빌드 도구 없는 순수 HTML/CSS/JS
- 백엔드/DB: Supabase (`SUPABASE_URL`, `SUPABASE_ANON_KEY`를 각 페이지 스크립트에서 직접 사용, publishable/anon 키라 커밋해도 무방)
- 디자인: `style.css`의 CSS 변수(`--coral`, `--coral-soft`, `--coral-bg` 등)로 코랄 톤 통일. 새 페이지를 추가할 때도 이 스타일시트를 링크해서 일관성 유지
- 모든 페이지는 상단에 동일한 `header.site-header` + `nav.site-nav` 구조를 사용 (홈/About/Todos 링크, 현재 페이지에 `active` 클래스)
- UI 문구는 한글 사용

## 폰트 규칙
- 폰트 컬러는 검정으로 통일한다.
- 폰트는 궁서체로 한다.