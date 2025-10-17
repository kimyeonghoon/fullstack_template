# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- 추가된 기능들을 여기에 나열

### Changed
- 변경된 기능들을 여기에 나열

### Deprecated
- 곧 제거될 기능들을 여기에 나열

### Removed
- 제거된 기능들을 여기에 나열

### Fixed
- 버그 수정 사항을 여기에 나열

### Security
- 보안 관련 변경사항을 여기에 나열

## [1.0.0] - 2025-01-17

### Added
- FastAPI 0.115.6 + Python 3.11 백엔드
- React Native 0.75+ + TypeScript 프론트엔드
- MySQL 8.0 데이터베이스
- Docker + Docker Compose 개발 환경
- JWT 인증 시스템 (Access + Refresh 토큰)
- 사용자 관리 API (회원가입, 로그인, 프로필)
- SQLAlchemy 2.0.36 ORM
- Pydantic v2 스키마 검증
- pytest 테스트 프레임워크 (커버리지 80%+)
- bcrypt 비밀번호 해싱
- WiFi 디버깅 지원
- CORS 미들웨어 설정
- 환경 변수 기반 설정 (.env)
- API 문서 자동 생성 (Swagger UI, ReDoc)

### Documentation
- README.md: 프로젝트 개요 및 시작 가이드
- CLAUDE.md: AI 협업 및 개발 규칙 (67개 규칙)
- docs/ARCHITECTURE.md: 시스템 아키텍처 다이어그램
- docs/DATABASE_SCHEMA.md: 데이터베이스 스키마 및 ER 다이어그램
- docs/TDD.md: 테스트 주도 개발 가이드
- docs/SECURITY.md: 보안 가이드
- docs/DEVELOPMENT.md: 개발 환경 설정 가이드
- docs/GETTING_STARTED.md: 신규 프로젝트 시작 가이드
- docs/WIFI_DEBUGGING.md: WiFi 디버깅 설정
- docs/WHY_DOCKER.md: Docker 개발의 필요성
- docs/VERSIONS.md: 패키지 버전 정보

### Infrastructure
- Docker 컨테이너 구성 (backend, frontend, mysql)
- Volume 마운트로 Hot Reload 지원
- MySQL 설정 파일 (my.cnf)
- pytest 테스트 환경 (SQLite)
- Pre-commit hooks 설정

### Security
- OWASP Top 10 대응
- SQL Injection 방지 (ORM 사용)
- 비밀번호 평문 저장 금지
- JWT 토큰 기반 인증
- 환경 변수로 민감 정보 관리
- 입력 검증 (Pydantic)
- CORS 설정

---

## 버전 규칙

이 프로젝트는 [Semantic Versioning](https://semver.org/)을 따릅니다:

- **MAJOR** (1.x.x): 호환되지 않는 API 변경
- **MINOR** (x.1.x): 하위 호환되는 기능 추가
- **PATCH** (x.x.1): 하위 호환되는 버그 수정

## 변경 내역 작성 규칙

### 카테고리

변경사항은 다음 카테고리로 분류합니다:

- **Added**: 새로운 기능 추가
- **Changed**: 기존 기능 변경
- **Deprecated**: 곧 제거될 기능 (하위 호환 유지)
- **Removed**: 제거된 기능 (Breaking Change)
- **Fixed**: 버그 수정
- **Security**: 보안 관련 변경

### 작성 예시

```markdown
## [1.1.0] - 2025-02-01

### Added
- 게시글 CRUD API 추가 (#12)
- 댓글 기능 구현 (#15)
- 파일 업로드 지원 (AWS S3) (#18)

### Changed
- JWT 토큰 만료 시간 변경: 30분 → 1시간 (#20)
- 사용자 프로필 응답 스키마 개선 (#22)

### Fixed
- 로그인 시 비활성 사용자 에러 메시지 개선 (#25)
- MySQL 연결 풀 설정 버그 수정 (#28)

### Security
- 비밀번호 해싱 알고리즘 강화 (bcrypt rounds: 12 → 14) (#30)
```

### Commit Message 연동

각 변경사항에는 관련 이슈 번호나 커밋을 연결합니다:
- `(#12)`: GitHub Issue 번호
- `(abc1234)`: Commit SHA

### 릴리스 날짜

모든 릴리스에는 날짜를 명시합니다 (ISO 8601: YYYY-MM-DD):
```markdown
## [1.2.0] - 2025-03-15
```

## 참고 자료

- [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
- [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
- [Conventional Commits](https://www.conventionalcommits.org/)
