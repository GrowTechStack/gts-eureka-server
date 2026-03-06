# GrowTechStack Eureka Server

마이크로서비스 인스턴스를 등록하고 위치를 관리하는 서비스 디스커버리 서버입니다.

## 기술 스택

| 분류 | 기술 |
|------|------|
| Language | Java 17 |
| Framework | Spring Boot 3.3.5 |
| Discovery | Spring Cloud Netflix Eureka Server |

## 주요 기능

- 마이크로서비스 자동 등록 및 해제 (heartbeat 기반)
- 등록된 인스턴스 헬스체크 및 상태 모니터링
- Gateway의 로드밸런싱(`lb://`)을 위한 서비스 위치 정보 제공

## 등록 서비스 목록

| 서비스 | 포트 |
|--------|------|
| gts-gateway | 8080 |
| gts-collector-service | 29999 |
| gts-ai-summary-service | 29998 |

## Eureka 대시보드

운영: `http://{EC2_IP}:8761`

## 배포

`main` 브랜치 push → GitHub Actions → ECR push → EC2 자동 배포
