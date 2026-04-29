---
description: RocketMQ consumer group
layout: schema
name: ConsumerGroup
properties_list:
- description: Consumer group name
  name: name
  type: string
- description: ''
  name: consumeFromWhere
  type: string
- description: ''
  name: consumeType
  type: string
- description: ''
  name: messageModel
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-consumer-group-schema.json
slug: apache-rocketmq-consumer-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-consumer-group-schema.json\",\n  \"title\": \"ConsumerGroup\",\n  \"description\": \"RocketMQ consumer group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer group name\"\n    },\n    \"consumeFromWhere\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONSUME_FROM_LAST_OFFSET\",\n        \"CONSUME_FROM_FIRST_OFFSET\",\n        \"CONSUME_FROM_TIMESTAMP\"\n      ]\n    },\n    \"consumeType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONSUME_ACTIVELY\",\n        \"CONSUME_PASSIVELY\"\n      ]\n    },\n    \"messageModel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BROADCASTING\",\n        \"CLUSTERING\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-consumer-group-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: ConsumerGroup
---
