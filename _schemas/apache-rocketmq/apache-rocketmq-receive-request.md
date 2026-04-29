---
description: Request to receive messages from a topic
layout: schema
name: ReceiveRequest
properties_list:
- description: Topic to consume from
  name: topic
  type: string
- description: Consumer group identifier
  name: consumerGroup
  type: string
- description: Maximum messages to pull
  name: maxMessages
  type: integer
- description: Invisible duration in milliseconds
  name: invisibleDuration
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-receive-request-schema.json
slug: apache-rocketmq-receive-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-receive-request-schema.json\",\n  \"title\": \"ReceiveRequest\",\n  \"description\": \"Request to receive messages from a topic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Topic to consume from\"\n    },\n    \"consumerGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer group identifier\"\n    },\n    \"maxMessages\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum messages to pull\"\n    },\n    \"invisibleDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Invisible duration in milliseconds\"\n    }\n  },\n  \"required\": [\n    \"topic\",\n    \"consumerGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-receive-request-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: ReceiveRequest
---
