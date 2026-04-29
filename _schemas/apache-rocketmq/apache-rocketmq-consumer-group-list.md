---
description: List of consumer groups
layout: schema
name: ConsumerGroupList
properties_list:
- description: ''
  name: groups
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-consumer-group-list-schema.json
slug: apache-rocketmq-consumer-group-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-consumer-group-list-schema.json\",\n  \"title\": \"ConsumerGroupList\",\n  \"description\": \"List of consumer groups\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groups\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConsumerGroup\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-consumer-group-list-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: ConsumerGroupList
---
