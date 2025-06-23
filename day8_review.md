# Day 8: AWS CLI + IAM 실습

## 개요
AWS CLI를 통해 IAM 사용자 생성, 정책 연결 및 S3/EC2 리소스 조회 실습을 수행함.

## 실습 내용
- S3 버킷 생성 및 삭제
- EC2 인스턴스 목록 조회
- IAM 사용자 생성 및 정책 연결
- CLI 결과 필터링 연습

## 주요 명령어

S3 버킷 생성 : aws s3 mb s3://jh-cli-test-bucket --region ap-northeast-2   
S3 버킷 삭제 : aws s3 rb s3://jh-cli-test-bucket --force
IAM 사용자 생성 : aws iam create-user --user-name cli-test-user
IAM 사용자 정책 연결 : aws iam attach-user-policy --user-name cli-test-user --policy-arn arn:aws:iam::aws:policy/AmazonS3ReadOnlyAccess
유저 리스트 목록 : aws iam list-users --query 'Users[*].UserName' --output table
