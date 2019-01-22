# kafka-docker-instance
using kafka docker instance to spin kafka consumer and producer with zookeeper 


Pull repo from 

git clone https://github.com/wurstmeister/kafka-docker

cd kafka-docker/

-> change the ports in docker-compose.yml file for kafka and zookeeper and also the host IP address. 

docker-compose up --build (to build docker image with new configurations)

->  to start producer 

$KAFKA_HOME/bin/kafka-console-producer.sh --topic=topic --broker-list=192.168.10.500:9095

-> to start consumer 

$KAFKA_HOME/bin/kafka-console-consumer.sh --topic=topic --bootstrap-server 192.168.10.500:9095

Bingo ! Go play with Kafka now :)
