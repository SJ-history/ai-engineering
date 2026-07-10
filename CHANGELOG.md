# Changelog

이 AI 엔지니어링 표준의 버전 이력. 형식은 [Keep a Changelog](https://keepachangelog.com/)를 따른다.

## [0.5.0]
### Added
- **검증자 분리(Maker ≠ Checker)** 개념 추가: 만드는 에이전트와 검사하는 에이전트를
  분리해 자기 채점 편향을 보정하는 기법을 `docs/03` 요소1에 반영.
- **루프의 구현 부품(5+1)** 신설: 오토메이션·워크트리·스킬·플러그인/커넥터·서브에이전트·
  상태 파일을 "루프가 실제로 무엇으로 구현되는가"의 체크리스트로 `docs/03` 요소6에 추가.
- **인지적 항복(Cognitive Surrender) 위험 신호** 추가: 루프가 매끄러워질수록 사람이
  결과물 이해를 포기하는 위험을 명시하고, 체크리스트·안티패턴 표에 반영.
- `templates/progress-template.md` 신설: 세션 간 이어지는 상태 파일 템플릿.
- `docs/06-glossary.md`에 검증자 분리·인지적 항복·상태 파일·오토메이션·워크트리·스킬 용어 추가.

### Changed
- `templates/task-loop-checklist.md`에 교차 검증·인지적 항복 점검·상태 파일 갱신 항목 추가.

## [0.4.0]
### Added
- **협업 경계(Collaboration Boundary) 원칙(P7)** 신설: 이 표준은 개인용이며, 팀에
  이미 규칙 파일(`CONTRIBUTING.md`, `CODEOWNERS` 등)이 있으면 그것이 정본이고
  `AGENTS.md`는 그 위의 개인 보충 레이어로만 얹는다는 원칙 명시.
- `templates/AGENTS.md`에 "0. 팀 표준과의 관계(정본 우선순위)" 절 추가 — 혼자 결정
  가능한 것과 팀 합의가 필요한 것의 경계, 충돌 시 처리 방법을 명문화.
- 에이전트 작업 규약에 "검증 결과를 PR·커밋 등 팀원도 보는 곳에 근거로 남긴다" 항목 추가
  — 개인 루프 실천을 협업 신뢰로 전환하는 지점.
- `docs/02-harness-engineering.md`(기둥1 컨텍스트, 기둥5 인터페이스), `docs/04-onboarding-playbook.md`
  (Phase 2)에 팀 규칙 우선 확인·병합 절차 반영.

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
