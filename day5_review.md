# 🚀 Day 5 – EC2 웹 페이지 자동 배포 실습

## 🔧 목표

- 로컬에서 작성한 HTML 파일(index.html)을 EC2 서버로 자동 전송
- 웹 브라우저에서 실시간으로 결과 확인

## ✅ 작업 절차

### 1. 로컬 HTML 파일 작성

```html
<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <title>EC2 배포</title>
</head>
<body>
  <h1>안녕하세요, 자동 배포 성공!</h1>
</body>
</html>

## EC2로 전송
# 방법 1: 바로 덮어쓰기 (sudo 권한 필요할 수 있음)
scp -i awsKeypair.pem index.html ec2-user@<EC2_IP>:/usr/share/nginx/html/

# 방법 2: 홈 디렉토리에 업로드 후 mv
scp -i awsKeypair.pem index.html ec2-user@<EC2_IP>:~/
ssh -i awsKeypair.pem ec2-user@<EC2_IP>
sudo mv ~/index.html /usr/share/nginx/html/

## 웹 브라우저 확인
http://<EC2 퍼블릭 IP>

## 특이사항
- 퍼미션 문제 발생시 sudo mv로 우회
- html 인코딩 설정 <meta charset="UTF-8"> 추가하여 한글깨짐 방지

## 느낀점
- 직접 배포하면서 퍼미션, 포트, 인코딩 문제를 실전처럼 다룸
- 서버와 클라이언트 간 배포 흐름을 이해할 수 있었음
- 실습 기반으로 CI/CD 흐름으로 확장할 수 있는 기반이 마련

