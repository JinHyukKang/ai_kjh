# /changelog

최근 변경 사항을 정리해 CHANGELOG.md에 기록한다.

## 동작 순서

1. 프로젝트 루트의 `CHANGELOG.md` 파일이 있으면 읽어 기존 항목을 파악한다.
2. `workspace/` 와 `calculator/` 디렉토리 내 HTML 파일들을 읽어 현재 상태를 파악한다.
3. 이번 대화에서 수행된 변경 사항(추가·수정·삭제)을 아래 형식으로 정리한다.
4. `CHANGELOG.md`를 생성하거나 업데이트한다 — 최신 항목이 파일 맨 위에 오도록 prepend한다.

## CHANGELOG.md 형식

```
# CHANGELOG

## [날짜] YYYY-MM-DD

### Added
- 새로 추가된 기능 또는 파일

### Changed
- 수정된 내용

### Fixed
- 버그 수정 내용

### Removed
- 삭제된 내용
```

변경 사항이 없는 항목(Added / Changed / Fixed / Removed)은 생략한다.
날짜는 오늘 날짜(currentDate)를 사용한다.
모든 내용은 한글로 작성한다.
