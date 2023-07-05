# Kafka

    1 - dowanload from  https://kafka.apache.org/downloads then unzip in c:\kafka
    2- make directory kafka-logs , zookeeper-data
    3- change server.properties    : log.dirs=c:/kafka/kafka-logs
    4- change zookeeper.properties : dataDir =c:/kafka/zookeeper-data
     
    5- run zookeeper-server-start.bat c:\kafka\config\zookeeper.properties or zookeeper-server-start.bat ../../config/zookeeper.properties
    6- run kafka-server-start.bat c:\kafka\config\server.properties or kafka-server-start.bat ../../config/server.properties 
    
    7- start a producer  cli : kafka-console-producer.bat --broker-list localhost:9092 --topic test
    8- start a consumer cli  : kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic test
