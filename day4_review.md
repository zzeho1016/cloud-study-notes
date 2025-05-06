# 📁 Day 4 – EC2 파일 전송 실습 (scp)

## 🔑 개념 요약

- `scp`: Secure Copy, SSH 기반 파일 복사 명령어
- 사용 목적: EC2 ↔ 로컬 간 파일 업로드/다운로드

## ✅ 명령어 예시

### 📤 로컬 → EC2 업로드

```bash
scp -i awsKeypair.pem hello.txt ec2-user@13.239.54.41:~/
