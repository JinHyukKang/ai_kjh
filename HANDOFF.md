# HANDOFF.md — 코드캠프 AI·머신러닝 아카데미 프로젝트

작성일: 2026-03-16

---

## 프로젝트 개요

**코드캠프(CodeCamp)** 브랜드의 AI·머신러닝 아카데미 홍보 사이트.
단일 HTML 파일 방식(HTML + `<style>` + `<script>` 일체형), 빌드 도구 없음.

---

## 파일 구조

```
ai_kjh/
├── CLAUDE.md              — Claude Code 프로젝트 지침
├── HANDOFF.md             — 이 파일
├── 머신러닝_프로젝트_PR.pdf — 강좌 기획 참고 문서
├── calculator/
│   └── index.html         — 3D 스타일 계산기 앱 (독립 프로젝트)
└── workspace/
    ├── index.html          — 메인 랜딩 페이지 (코드캠프 홈)
    └── courses.html        — ML 프로젝트 강좌 상세 페이지
```

---

## 완성된 결과물

### `workspace/index.html` — 메인 랜딩 페이지

| 섹션 | 내용 |
|------|------|
| **Navigation** | 고정 상단 바, 스크롤 시 blur 배경, 모바일 햄버거 메뉴 |
| **Hero** | 풀스크린, 마우스 패럴랙스 orb 효과, 스크롤 reveal 애니메이션 |
| **Stats** | 누적 수강생·만족률·강좌 수·만족도 숫자 카운터 애니메이션 |
| **Courses** | 4단계 ML 프로젝트 로드맵 카드 (Step 1~4) |
| **Features** | 교육 방식 설명 + 2×2 feature 카드 |
| **Reviews** | 수강생 후기 3개 카드 |
| **CTA Banner** | 선행 과정 안내 + 상담 신청/전화 버튼 |
| **Footer** | 브랜드·강좌·회사·지원 4열 그리드 |

**주요 JS 기능:**
- 스크롤 navbar 상태 전환 (`scrolled` 클래스)
- 모바일 햄버거 메뉴 토글
- 앵커 스무스 스크롤 (navbar 높이 80px 오프셋)
- IntersectionObserver 기반 스크롤 reveal
- 숫자 카운터 애니메이션 (easeOutCubic)
- 마우스무브 Hero 패럴랙스

### `workspace/courses.html` — 강좌 상세 페이지

메인 랜딩과 동일한 디자인 시스템(CSS 변수·컴포넌트) 적용.
커리큘럼 상세, 수강 신청 등 상세 정보 페이지.

### `calculator/index.html` — 3D 계산기

별도 독립 프로젝트. 3D CSS 스타일 계산기 앱.

---

## 디자인 시스템

| 변수 | 값 |
|------|----|
| `--clr-primary` | `#6C63FF` (보라) |
| `--clr-accent` | `#06B6D4` (시안) |
| `--clr-accent-warm` | `#F59E0B` (앰버) |
| `--clr-bg` | `#0F0F1A` (다크) |
| `--clr-bg-card` | `#1A1A2E` |
| `--clr-muted` | `#94a3b8` |
| `--radius` | `12px` |

- 레이아웃: CSS Grid + Flexbox
- 반응형 브레이크포인트: 1024px / 768px / 480px
- 폰트: Segoe UI / system-ui

---

## 실행 방법

빌드 불필요. `workspace/index.html` 또는 `calculator/index.html`을 브라우저에서 직접 열면 됨.

---

## 다음 작업 후보

- `courses.html` 커리큘럼 섹션 콘텐츠 보강
- 수강 신청 폼 기능 추가 (validation 포함)
- `calculator/` 기능 확장
