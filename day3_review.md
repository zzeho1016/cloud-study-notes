# 🌐 Day 3 – EC2에서 Nginx 웹 서버 구성 실습

## 🔧 Nginx 개요

- 오픈소스 고성능 웹 서버
- 정적 파일 제공, 리버스 프록시, 로드 밸런서 기능 포함
- 이벤트 기반 처리 구조로 Apache보다 경량화됨

## ✅ 설치 및 실행

```bash
sudo dnf update -y
sudo dnf install nginx -y
sudo systemctl start nginx
sudo systemctl enable nginx  # 선택
sudo systemctl status nginx  # 상태 확인

