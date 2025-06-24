# Day 9: AWS CloudWatch Logs 실습

## 목표
CloudWatch를 통해 로그 그룹, 로그 스트림을 생성하고 로그 이벤트를 삽입 및 조회하는 CLI 실습 진행.

## 명령어 요약

```bash
aws logs create-log-group --log-group-name my-cloudwatch-group
aws logs create-log-stream --log-group-name my-cloudwatch-group --log-stream-name my-stream

TIMESTAMP=$(date +%s%3N)
aws logs put-log-events --log-group-name my-cloudwatch-group --log-stream-name my-stream \
  --log-events timestamp=$TIMESTAMP,message="Hello from CloudWatch CLI"

aws logs get-log-events --log-group-name my-cloudwatch-group --log-stream-name my-stream --limit 5

aws logs delete-log-group --log-group-name my-cloudwatch-group
