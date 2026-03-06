# GrowTechStack Eureka Server

마이크로서비스 간의 위치를 파악하고 관리하는 서비스 디스커버리 서버입니다.

## 기술 스택

| 분류 | 기술 |
|------|------|
| Language | Java 17 |
| Framework | Spring Boot 3.3.5 |
| Discovery | Spring Cloud Netflix Eureka Server |

## 주요 기능

- 서비스 등록 및 해제 관리
- 등록된 인스턴스 상태 모니터링
- 서비스 위치(IP, Port) 정보 제공

## 환경 변수

| 변수 | 설명 |
|------|------|
| `SERVER_PORT` | 서버 포트 (기본: 8761) |

## 로컬 개발

```bash
./gradlew bootRun
```
Dashboard: `http://localhost:8761`
