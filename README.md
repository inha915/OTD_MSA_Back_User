# 👤 OTD_MSA_Back_User

**OneToday (OTD)** 백엔드 **유저 서비스(User Service)** 레포지토리입니다.  
이 서비스는 MSA(Microservice Architecture) 구조에서 **회원, 인증, 프로필, 포인트, 알림** 등의 사용자 도메인을 담당합니다.

---

## ⚙️ 기술 스택

| 항목 | 내용 |
|------|------|
| 언어 | Java 17 |
| 프레임워크 | Spring Boot 3.x |
| ORM | Spring Data JPA |
| 보안 | Spring Security, JWT |
| DB | MariaDB |
| 빌드도구 | Gradle |
| 배포환경 | Docker, Kubernetes |

---

## 🚀 실행 방법

```bash
# 1) 애플리케이션 실행
./gradlew bootRun

---

💡 주요 기능
🧾 회원가입 / 로그인 / 로그아웃
🔐 JWT 기반 인증 및 인가
👤 사용자 정보 조회 및 수정
💰 포인트 적립 및 관리
🔔 알림 기능 (게이트웨이 연동 예정)

---

🧠 서비스 아키텍처

[Gateway]
   ↓
[OTD_MSA_Back_User]
   ↓
[User DB / Redis / Notification Queue]
