---
description: Request to send a message to RocketMQ
layout: schema
name: MessageRequest
properties_list:
- description: Target topic name
  name: topic
  type: string
- description: Message body content
  name: body
  type: string
- description: Message tag for filtering
  name: tag
  type: string
- description: Message keys for lookup
  name: keys
  type: array
- description: User-defined message properties
  name: properties
  type: object
- description: Delay level for scheduled messages (0=no delay)
  name: delayLevel
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-message-request-schema.json
slug: apache-rocketmq-message-request
source_filename: apache-rocketmq-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-message-request-schema.json\",\n  \"title\": \"MessageRequest\",\n  \"description\": \"Request to send a message to RocketMQ\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Target topic name\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Message body content\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Message tag for filtering\"\n    },\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Message keys for lookup\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"User-defined message properties\"\n    },\n    \"delayLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Delay level for scheduled messages (0=no delay)\"\n    }\n  },\n  \"required\": [\n    \"topic\",\n    \"body\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-message-request-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: MessageRequest
---
