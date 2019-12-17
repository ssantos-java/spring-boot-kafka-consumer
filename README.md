# Spring Boot with Kafka Consumer Example

Este projeto cobre o uso do Spring Boot com Spring Kafka para consumir JSON/String mensagens de um Kafka topic
## Iniciando Zookeeper
- `bin/zookeeper-server-start.sh config/zookeeper.properties`

## Iniciando Kafka Server
- `bin/kafka-server-start.sh config/server.properties`

## Criando Kafka Topic
- `bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example`
- `bin/kafka-topics.sh --create --zookeeper localhost:2181 --replication-factor 1 --partitions 1 --topic Kafka_Example_json`

## Publicando to the Kafka Topic via Console
- `bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example`
- `bin/kafka-console-producer.sh --broker-list localhost:9092 --topic Kafka_Example_json`
