# EFK
Elasticsearch + Fluentd + Kibana

## 테스트 과정

1. docker-compose 실행
```shell
docker-compose up
```

2. 테스트 데이터 준비
```shell
cat test.json

{"message":{"data":"test_bong_u"}}
```

3. 테스트 데이터 전송
```shell
nc localhost 24224 < test.json
```

4. kibana에서 결과 확인
![image](https://user-images.githubusercontent.com/68285620/220658955-a85e3a69-f5f6-4f9b-bbb8-c218d294b7b0.png)
