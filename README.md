# kafka
##kafka fundamentals

### Producer

To get data into a kafka cluster, we have a thing called producer. A producer is an application that you write

### Consumer

### Broker

### Zookeeper

### Topic

### Partition

### Record

### Replication factor (Partitions)

### Commands

start-kafka

```shell
bin/zookeeper-server-start.sh config/zookeeper.properties
bin/kafka-server-start.sh config/server.properties
```

stop-kafka

```shell
bin/kafka-server-stop.sh config/server.properties
bin/zookeeper-server-stop.sh config/zookeeper.properties
```
describe topics

```shell
bin/kafka-topics.sh --describe --topic topic-name --bootstrap-server locahost:9092
```

list-topics

```shell
bin/kafka-topics.sh --list --bootstrap-server localhost:9092
```

create-consumer

```shell
bin/kafka-console-consumer.sh --topic topic-name --from-beginning --boostrap-server localhost:9092
```

create-topic

```shell
bin/kafka-topic.sh --create --zookeeper localhost:2181 --repication-factor 1 --partitions 1 --topic topic-name
```

delete-topic

```shell
bin/kafka-topic.sh --delete --zookeeper localhost:2181 --topic topic-name
```

create-producer

```shell
bin/kafka-console-producer.sh --topic topic-name --bootstrap-server localhost:9092
```
