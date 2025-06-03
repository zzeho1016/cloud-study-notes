# Day 7: S3 정적 웹사이트 호스팅 실습

## 개요
AWS S3를 활용해 EC2 없이 정적 웹사이트를 배포해보는 실습입니다.

## 실습 내용
- 버킷 생성
- 정적 웹 호스팅 활성화
- index.html 업로드
- 퍼블릭 접근 허용 (버킷 정책 설정)

## 명령어 예시
```bash
echo "<h1>Hello from S3</h1>" > index.html
aws s3 cp index.html s3://jh-static-web-2025/
