# kafkaSample
Apache Kafka, Spring Boot를 사용한 Sample 예제입니다.

# 아파치 카프카 명령어
주키퍼 실행 & 중지

bin/zookeeper-server-start.sh config/zookeeper.properties

bin/zookeeper-server-stop.sh


카프카 실행 & 중지

bin/kafka-server-start.sh config/server.properties

bin/kafka-server-stop.sh


토픽(test) 생성

bin/kafka-topics.sh --create --bootstrap-server localhost:9092 --replication-factor 1 --partitions 3 --topic test


프로듀서 실행

bin/kafka-console-producer.sh --bootstrap-server localhost:9092 --topic test


컨슈머 실행

bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic test --from-beginning
