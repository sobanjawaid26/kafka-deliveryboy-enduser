Start Zookeeper
- bin/zookeeper-server-start.sh config/zookeeper.properties


Start Kafka
- bin/kafka-server-start.sh config/server.properties


Create topic
- bin/kafka-topics.sh --create --topic location-update-topic --bootstrap-server localhost:9092


Write event into Topic
- bin/kafka-console-producer.sh --topic location-update-topic --bootstrap-server localhost:9092


Consume Topic
- bin/kafka-console-consumer.sh --topic location-update-topic --from-beginning --bootstrap-server localhost:9092
