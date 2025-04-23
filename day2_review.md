# 🖥️ Day 2 – EC2 실습 정리

## 1. EC2 개요
- AWS에서 제공하는 가상 머신 서비스
- 프리 티어: t2.micro (750시간/월 무료)

## 2. 인스턴스 생성 절차
- Amazon Linux 2023 선택
- 키 페어 생성 및 `.pem` 다운로드
- 보안 그룹에서 SSH(22) 허용
- 퍼블릭 IP 확인

## 3. SSH 접속

```bash
chmod 400 my-key.pem
ssh -i my-key.pem ec2-user@<public-ip>

