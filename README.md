## General info

Replace `.bat` scripts below by their corresponding `.sh` scripts if running under linux.

## Start Zookeeper server

`
.\zookeeper-server-start.bat ..\..\config\zookeeper.properties
`

## Start Kafka bootstrap server

`
.\kafka-server-start.bat ..\..\config\server.properties
`

## Create kafka topic

`
.\kafka-topics.bat --topic ecommerce_new_order --bootstrap-server localhost:9092 --create
`

## Start consumer

`
.\kafka-console-consumer.bat --boostrap-server localhost:9092 --topic ecommerce_new_order
`