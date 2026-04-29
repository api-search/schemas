---
description: Received RocketMQ message
layout: schema
name: Message
properties_list:
- description: Message identifier
  name: msgId
  type: string
- description: Topic name
  name: topic
  type: string
- description: Message body
  name: body
  type: string
- description: Message tag
  name: tag
  type: string
- description: ''
  name: keys
  type: array
- description: ''
  name: properties
  type: object
- description: Message creation timestamp in milliseconds
  name: bornTimestamp
  type: integer
- description: Handle for acknowledging the message
  name: receiptHandle
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-message-schema.json
slug: apache-rocketmq-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-message-schema.json\",\n  \"title\": \"Message\",\n  \"description\": \"Received RocketMQ message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"msgId\": {\n      \"type\": \"string\",\n      \"description\": \"Message identifier\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Topic name\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Message body\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Message tag\"\n    },\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"bornTimestamp\"\
  : {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Message creation timestamp in milliseconds\"\n    },\n    \"receiptHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Handle for acknowledging the message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-message-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Message
---
