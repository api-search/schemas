---
description: List of RocketMQ topics
layout: schema
name: TopicList
properties_list:
- description: ''
  name: topics
  type: array
- description: ''
  name: total
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-topic-list-schema.json
slug: apache-rocketmq-topic-list
source_filename: apache-rocketmq-topic-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-list-schema.json\",\n  \"title\": \"TopicList\",\n  \"description\": \"List of RocketMQ topics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Topic\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-list-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TopicList
---
