# 패키지 버전 정보

이 문서는 템플릿에서 사용하는 모든 주요 패키지의 버전 정보를 포함합니다.

## 백엔드 (Python)

### 코어 프레임워크
- **Python**: 3.11+
- **FastAPI**: 0.115.6
- **Uvicorn**: 0.34.0
- **Gunicorn**: 23.0.0

### 데이터베이스
- **SQLAlchemy**: 2.0.36
- **PyMySQL**: 1.1.1
- **MySQL**: 8.0+

### 인증 및 보안
- **python-jose[cryptography]**: 3.3.0
- **passlib[bcrypt]**: 1.7.4
- **cryptography**: 44.0.0

### 데이터 검증
- **Pydantic**: 2.10.3
- **pydantic-settings**: 2.7.0
- **email-validator**: 2.2.0

### 기타
- **python-multipart**: 0.0.20 (파일 업로드)
- **python-dotenv**: 1.0.1 (환경 변수)

## 프론트엔드 (JavaScript/TypeScript)

### 코어
- **Node.js**: 20+ (LTS)
- **React Native**: 최신 버전 (0.75+)
- **TypeScript**: 최신 버전 (5.x)

### UI 라이브러리
- **react-native-paper**: 5.12.5
- **react-native-vector-icons**: 10.2.0
- **react-native-safe-area-context**: 4.14.0

### 네비게이션
- **@react-navigation/native**: 6.1.18
- **@react-navigation/stack**: 6.4.1
- **@react-navigation/bottom-tabs**: 6.6.1
- **react-native-screens**: 3.34.0
- **react-native-gesture-handler**: 2.20.2

### 데이터 및 상태 관리
- **axios**: 1.7.9
- **@react-native-async-storage/async-storage**: 2.1.0

## 개발 도구

### 백엔드
- **pytest**: 최신 버전 (테스트)
- **pytest-asyncio**: 최신 버전 (비동기 테스트)
- **httpx**: 최신 버전 (API 테스트)
- **alembic**: 최신 버전 (데이터베이스 마이그레이션)

### 프론트엔드
- **Metro**: React Native 기본 번들러
- **ESLint**: 코드 린팅
- **Prettier**: 코드 포맷팅

## 인프라

### 컨테이너
- **Docker**: 20.10+
- **Docker Compose**: 2.0+

### 데이터베이스
- **MySQL**: 8.0

## 버전 업데이트 주기

이 템플릿은 다음 일정으로 업데이트됩니다:

- **주요 버전 업데이트**: 분기별 (3개월)
- **마이너 버전 업데이트**: 월별
- **보안 패치**: 즉시

## 호환성 매트릭스

### Python 버전
- Python 3.11, 3.12 호환 확인됨

### Node.js 버전
- Node.js 20 LTS 권장
- Node.js 18 LTS 호환

### React Native 버전
- 0.75.x 테스트 완료
- 0.74.x 호환 가능

## 중요 변경사항

### 2025년 1월 업데이트

**백엔드:**
- FastAPI 0.115.6으로 업데이트 (이전: 0.109.0)
- Pydantic 2.10.3으로 업데이트 - `model_config` 사용
- SQLAlchemy 2.0.36으로 업데이트
- Uvicorn 0.34.0으로 업데이트
- cryptography 명시적 추가 (44.0.0)

**프론트엔드:**
- React Native Paper 5.12.5
- React Navigation 6.1.18
- Axios 1.7.9
- TypeScript 타입 안전성 개선

### 주요 변경사항 상세

#### Pydantic v2 마이그레이션
- `Config` 클래스 → `model_config` (SettingsConfigDict)
- `@computed_field` 데코레이터 추가
- 타입 힌트 개선

#### React/TypeScript 개선
- `useCallback`, `useMemo` 훅 추가로 성능 최적화
- Axios 타입 정의 개선
- 더 엄격한 타입 체크

## 다음 업데이트 예정

### 백엔드
- [ ] Alembic 마이그레이션 예제 추가
- [ ] 테스트 코드 템플릿 추가
- [ ] Redis 캐싱 예제 추가

### 프론트엔드
- [ ] 상태 관리 라이브러리 추가 (Zustand/Redux)
- [ ] 오프라인 지원 예제
- [ ] 푸시 알림 설정

## 문의

버전 관련 문제나 제안사항이 있으시면 GitHub Issues에 등록해주세요.
