# spring-cloud-streams-kafka-demo
Sample application using Spring Boot, Spring Cloud Stream and Kafka. https://dzone.com/articles/spring-cloud-stream-with-kafka

Forked from David Kiss. Why do not you let me send a raw json in the message, David? :) It is coded to use a String as payload, 
it should work with json content. If you try to run this in local mode, you have to put this line at 

aironman$ sudo vim /usr/local/etc/kafka/server.properties

...
offsets.topic.replication.factor=1

