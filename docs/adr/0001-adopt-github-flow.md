# 0001. GitHub Flow 도입

날짜: 2026-11-09

## Status

Accepted

## Context

이 레포는 혼자 또는 소규모로 작업하며 변경 사항을 지속적으로 `main`에 반영한다. 이전에는 `main`에 직접 커밋해 왔다.

## Decision

GitHub Flow를 채택한다. `main`을 기준 브랜치로 유지하고, `feature/*` 등 작업 브랜치에서 변경한 뒤 Pull Request 리뷰를 거쳐 squash 머지한다. 커밋 메시지에는 Conventional Commits 형식을 사용한다.

## Consequences

장점:
- 작업과 변경 이력을 추적하기 쉽다.
- Pull Request에 리뷰 기록이 남는다.
- 머지 전에 CI 검증 결과를 확인할 수 있다.

단점:
- 브랜치 생성, Pull Request 작성과 리뷰 등 작업 절차가 늘어난다.
