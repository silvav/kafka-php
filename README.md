# Kafka PHP
Running Kafka on Docker with PHP client for producing and consuming messages.

## Testing Kafka setup
Testing the kafka server via the CLI.

Steps taken from the [Apache Kafka Quickstart](https://kafka.apache.org/quickstart).

### Create a topic to store events
```shell
/usr/bin/kafka-topics --create --topic quickstart-events --bootstrap-server localhost:9092
```

Show topic details
```shell
/usr/bin/kafka-topics --describe --topic quickstart-events --bootstrap-server localhost:9092
```

### Write some events into the topic
```shell
/usr/bin/kafka-console-producer --topic quickstart-events --bootstrap-server localhost:9092
>my first event
>my second event
```
crtl+c to stop 

### Read the events
```shell
/usr/bin/kafka-console-consumer --topic quickstart-events --from-beginning --bootstrap-server localhost:9092
```
crtl+c to stop

## Rdkafka examples

[Example using the RdKafka extension that provides a Kafka client for PHP](https://arnaud.le-blanc.net/php-rdkafka-doc/phpdoc/rdkafka.examples.html).
