## 기술 스택
Backend:
- Java 21 (LTS) - 가상 스레드, 패턴 매칭 등 최신 기능 활용
- Spring Boot 3.3.x - Java 21 완벽 지원, 최신 보안 패치
- Spring Data JPA 3.3.x - Spring Boot와 호환
- Netty 4.1.x - 안정성과 성능이 검증된 버전
- Spring WebSocket 6.1.x - Spring Boot 3.3과 호환
- Redis 7.2.x - 최신 안정 버전, 성능 개선
- MySQL 8.0.x - JSON 지원, 성능 최적화

DevOps:
- Docker 24.x - 최신 기능 지원
- Prometheus 2.50.x + Grafana 10.x - 최신 모니터링 기능
- GitHub Actions - 클라우드 기반 CI/CD

## 프로젝트 구조
youtube-watch-together/
├── backend/
│   ├── src/main/java/com/watchTogether/
│   │   ├── config/          # 설정 클래스
│   │   ├── controller/      # REST API
│   │   ├── websocket/       # WebSocket 핸들러
│   │   ├── netty/          # Netty 서버 구현
│   │   ├── service/        # 비즈니스 로직
│   │   ├── repository/     # 데이터 접근
│   │   ├── entity/         # JPA 엔티티
│   │   ├── dto/            # 데이터 전송 객체
│   │   ├── exception/      # 예외 처리
│   │   └── util/           # 유틸리티
│   ├── src/main/resources/
│   └── pom.xml or build.gradle
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── monitoring/
│   ├── prometheus/
│   └── grafana/
└── .github/workflows/
