# Changelog

이 AI 엔지니어링 표준의 버전 이력. 형식은 [Keep a Changelog](https://keepachangelog.com/)를 따른다.

## [0.3.0]
### Changed
- **단일 규칙 파일(One Rules File) 원칙 확립**: 도구별 어댑터/규칙 파일 체계를 폐기.
  규칙 정본은 `templates/AGENTS.md` 하나이며, 이를 읽지 못하는 에이전트는
  한 줄짜리 포인터 파일로만 연결한다(본문 복제 금지).
- README를 "새 환경 3단계 세팅(모든 IDE·에이전트 공통)" 중심으로 재작성.

### Removed
- `templates/adapters/` (도구별 어댑터 4종) — 환경마다 파일이 갈라져 관리 지점이
  늘어나는 문제로 폐기.

## [0.2.0]
### Changed
- 도구 종속 구조(`cursor-rule.mdc`)를 제거하고 도구 비종속 표준으로 재설계.
- 얕은 단일 README를 **이론(docs) + 산출물(templates)** 구조로 분리.

### Added
- `docs/`: 프레임워크(01), 하네스(02), 루프(03), 온보딩 플레이북(04), 성숙도 모델(05), 용어집(06).
- `templates/`: `AGENTS.md`, 작업 루프 체크리스트, 검증 매트릭스.
- 성숙도 모델(L0–L4)과 자가진단 매트릭스.

## [0.1.0]
### Added
- 최초 버전: `AGENTS.md`, `cursor-rule.mdc`, `work-loop-checklist.md`, `README.md`.
- 하네스/루프 개념과 기본 템플릿 도입.
