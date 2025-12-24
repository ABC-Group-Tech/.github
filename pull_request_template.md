# Pull Request 제목 규칙 (PR Title Rules)

## 1. 목적
본 문서는 Pull Request(PR) 제목을 **일관되고 명확하게 작성**하여  
다음 목적을 달성하기 위해 정의한다.

- PR 목록에서 변경 의도를 즉시 파악
- 커밋/릴리즈 노트 자동화 용이
- 리뷰 비용 감소
- AI 기반 개발 시 변경 책임 추적 명확화

<!-- PR Title Template -->
## 2. 기본 제목 형식 (필수)

PR 제목은 아래 형식을 **반드시** 따른다.

[type(scope)] 한 줄 요약 또는 type(scope): 한 줄 요약
예: feat(order): 자동 발주 생성 로직 추가

**type 예시**
- feat 기능
- fix 버그
- refactor 리팩토링(동작 동일)
- perf 성능
- test 테스트
- docs 문서
- chore 설정/잡무(빌드, CI, deps 등)

**scope 예시**
- UI
- Domain(Order, Cart, User....)
- schema

<!-- PR Body Template -->
## 1. 요약 (Summary)
- 무엇을 변경했는지 2~3줄로 요약

## 2. 배경/문제 (Context)
- 왜 이 변경이 필요한가?
- 관련 이슈/티켓: (Notion 링크)

## 3. 변경 내용 (Changes)
- [ ] 주요 변경 1
- [ ] 주요 변경 2
- [ ] 주요 변경 3

## 4. 영향 범위 (Impact)
- 영향 받는 모듈/서비스:
  - apps/...
  - packages/...
- DB/Schema 변경 여부: Yes/No (마이그레이션 포함 여부)

## 5. 검증 (Verification)
### 자동 테스트
- [ ] unit
- [ ] e2e
