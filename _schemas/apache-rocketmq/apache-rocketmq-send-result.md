---
description: Result of sending a message
layout: schema
name: SendResult
properties_list:
- description: Message identifier
  name: msgId
  type: string
- description: Physical offset message ID
  name: offsetMsgId
  type: string
- description: Queue offset of the message
  name: queueOffset
  type: integer
- description: Queue ID the message was sent to
  name: queueId
  type: integer
- description: ''
  name: sendStatus
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-send-result-schema.json
slug: apache-rocketmq-send-result
source_filename: apache-rocketmq-send-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-send-result-schema.json\",\n  \"title\": \"SendResult\",\n  \"description\": \"Result of sending a message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"msgId\": {\n      \"type\": \"string\",\n      \"description\": \"Message identifier\"\n    },\n    \"offsetMsgId\": {\n      \"type\": \"string\",\n      \"description\": \"Physical offset message ID\"\n    },\n    \"queueOffset\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Queue offset of the message\"\n    },\n    \"queueId\": {\n      \"type\": \"integer\",\n      \"description\": \"Queue ID the message was sent to\"\n    },\n    \"sendStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SEND_OK\",\n        \"FLUSH_DISK_TIMEOUT\",\n        \"FLUSH_SLAVE_TIMEOUT\"\
  ,\n        \"SLAVE_NOT_AVAILABLE\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-send-result-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: SendResult
---
