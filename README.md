# spring-cloud-streams-kafka-demo
Sample application using Spring Boot, Spring Cloud Stream and Kafka. https://dzone.com/articles/spring-cloud-stream-with-kafka

Forked from David Kiss. Why do not you let me send a raw json in the message, David? :) It is coded to use a String as payload, 
it should work with json content. If you try to run this in local mode, you have to put this line at the end of the file server.properties:

$ sudo vim /usr/local/etc/kafka/server.properties


offsets.topic.replication.factor=1

Then, you must run zookeeper:

$ zookeeper-server-start /usr/local/etc/kafka/zookeeper.properties

next, you must run kafka:

$ kafka-server-start /usr/local/etc/kafka/server.properties

Then, you can run the project after you clone the code in a folder with mvn spring-boot:run, then go to http://localhost:8080/greetings?message=JSON

and check the kafka's terminal.

Thanks David.
