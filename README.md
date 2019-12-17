# Kafka-Connect-Plugin-Examples
Plugin Examples

## MySQL JDBC Source Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## MySQL JDBC Sink Connector
```
{
	"name": "mysink",
	"config": {
		"connector.class": "io.confluent.connect.jdbc.JdbcSinkConnector",
		"connection.password": "dddd",
		"errors.tolerance":"all",
		"errors.deadletterqueue.context.headers.enable":true,
		"errors.deadletterqueue.topic.name": "mytest_cust_fraud",
		"errors.log.enable": true,
    "errors.log.include.messages": true,
		"topics": "mytest_cust_fraud",
		"connection.user": "ddd",
		"name": "mysink",
		"auto.create": "true",
		"connection.url": "jdbc:mysql://edpnew.c7uqx6xqd0nl.us-east-1.rds.amazonaws.com:3306/myexplore",
		"insert.mode": "insert"
	}
}
```

## RabbitMQ Source Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## JMS Source Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## S3 Sink Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## MongoDB Source Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## MongoDB Sink Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}

```
## Splunk Sink Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## Snowflake Sink Connector
```
{
  "name": "snow",
  "connector.class": "com.snowflake.kafka.connector.SnowflakeSinkConnector",
  "tasks.max": "1",
  "key.converter": "org.apache.kafka.connect.storage.StringConverter",
  "value.converter": "com.snowflake.kafka.connector.records.SnowflakeJsonConverter",
  "transforms": "",
  "topics": [
    "my_cust_json"
  ],
  "snowflake.url.name": "xxx.us-east-1.snowflakecomputing.com",
  "snowflake.user.name": "xxx",
  "snowflake.private.key": "xxx",
  "snowflake.private.key.passphrase": "snowflake",
  "snowflake.database.name": "DEMO_DB",
  "snowflake.schema.name": "MYTESTSCHEMA",
  "snowflake.topic2table.map": "my_test_topic:MY_TEST_TABLE"
}
```

## Elasticsearch Sink Connector
```
{
  "name": "elasticsearch-sink",
  "config": {
    "connector.class": "io.confluent.connect.elasticsearch.ElasticsearchSinkConnector",
    "tasks.max": "1",
    "topics": "test-topic",
    "key.ignore": "true",
    "connection.url": "http://localhost:9200",
    "type.name": "kafka-connect",
    "name": "elasticsearch-sink"
  }
}
```
