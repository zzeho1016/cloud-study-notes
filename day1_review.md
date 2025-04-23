# 📘 AWS 기본 개념 요약

---

### 1. ☁️ 클라우드 컴퓨팅 개요

- **클라우드 컴퓨팅 정의**  
  인터넷을 통해 서버, 저장소, 데이터베이스, 네트워킹, 소프트웨어 등 IT 자원을 **온디맨드(On-demand)** 방식으로 제공하는 기술

- **3가지 서비스 모델**

| 서비스 | 설명                           | 예시                  |
| ------ | ------------------------------ | --------------------- |
| IaaS   | 인프라(서버, 스토리지 등) 제공 | Amazon EC2, S3        |
| PaaS   | 플랫폼(개발 환경) 제공         | AWS Elastic Beanstalk |
| SaaS   | 완성된 소프트웨어 제공         | Gmail, Dropbox        |

---

### 2. 🔑 AWS 글로벌 인프라 구조

- **리전(Region)**: 서로 다른 지리적 위치, 예: 서울 리전(ap-northeast-2)
- **가용 영역(Availability Zone, AZ)**: 하나의 리전 내 여러 데이터센터
- **엣지 로케이션(Edge Location)**: 콘텐츠를 사용자에게 빠르게 전송 (CDN용)

---

### 3. 🧰 AWS 핵심 서비스 요약

| 서비스                               | 설명                           |
| ------------------------------------ | ------------------------------ |
| EC2 (Elastic Compute Cloud)          | 가상 서버 생성 서비스          |
| S3 (Simple Storage Service)          | 객체 스토리지, 파일 저장       |
| RDS (Relational Database Service)    | 관리형 관계형 데이터베이스     |
| IAM (Identity and Access Management) | 사용자/권한 관리               |
| VPC (Virtual Private Cloud)          | 가상 네트워크 환경 구성        |
| Lambda                               | 서버 없이 코드 실행 (서버리스) |
| CloudWatch                           | 로그 및 성능 모니터링          |
| Route 53                             | DNS 서비스                     |

---

### 4. 🛡️ 보안과 관리

- **IAM**: 사용자/그룹/역할(Role) 정의, 최소 권한 원칙
- **CloudTrail**: 모든 API 호출 로그 기록
- **KMS (Key Management Service)**: 데이터 암호화 키 관리

---

### 5. 💰 과금 방식 & 가격 구조

- **종량 과금(Pay as you go)**: 사용한 만큼만 비용 청구
- **프리 티어(Free Tier)**: 신규 사용자 12개월 동안 무료 서비스 제공
- **요금 계산기**: [AWS 가격 계산기](https://calculator.aws.amazon.com/)

---

### 6. 📝 AWS Cloud Practitioner 시험 영역

| 영역              | 비중 |
| ----------------- | ---- |
| 클라우드 개념     | 26%  |
| 보안 및 규정 준수 | 25%  |
| 기술적 설명       | 33%  |
| 결제 및 지원      | 16%  |

---

### 🧠 추가 팁

- Cloud Practitioner는 실습보다 **개념 중심** 공부
- 각 서비스별 **사용 사례(use case)** 위주로 기억하면 유리
