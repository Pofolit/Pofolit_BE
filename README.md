### 개발 환경 (Development Environment)
- **Java 17**, **Spring Boot 3.4.7** , **Gradle-jar**
- IDE: **IntelliJ IDEA**
- Management process: **Notion** _sprint_style_
- Database: { **MySQL** }
- CI/CD: { **GitHub Actions**, **Docker** } 
- Dependencies:
  - JPA , mapstruct , flyway-core 
  - Spring-Security ,  JWT 12.6 , OAuth2: _kakao,google_
  - JUnit , Mockito
  - Swagger-ui

> backend port : http://localhost:8080/    
> frontend port : http://localhost:3000/
 
---
### 디렉토리 구조
domain-layer style
```text
com.app.pofolit_be
  ├── ...
  │   ├── ...          
  ├── userDomain          
  │   ├── controller/      // API 엔드포인트 컨트롤러
  │   ├── dto/             // DTO (Data Transfer Objects)
  │   ├── entity/          // Entity classes
  │   ├── mapper/          // MapStruct 매퍼 인터페이스
  │   ├── repository/      // JPA 리포지토리 인터페이스
  │   ├── service/         // 도메인 서비스 인터페이스
  │   └── useCase/         // 도메인 서비스 구현체
  └── config              
      ├── security/        // JWT, OAuth2 등 보안 관련 코드  설정      
      ├── exceptions/      // 예외 + 핸들러
      └── utils/           // 공통 유틸리티 클래스
```

