---
description: Request to acknowledge a message
layout: schema
name: AckRequest
properties_list:
- description: Receipt handle from receive response
  name: receiptHandle
  type: string
- description: Topic name
  name: topic
  type: string
- description: Consumer group
  name: consumerGroup
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-ack-request-schema.json
slug: apache-rocketmq-ack-request
source_filename: apache-rocketmq-ack-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-ack-request-schema.json\",\n  \"title\": \"AckRequest\",\n  \"description\": \"Request to acknowledge a message\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"receiptHandle\": {\n      \"type\": \"string\",\n      \"description\": \"Receipt handle from receive response\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Topic name\"\n    },\n    \"consumerGroup\": {\n      \"type\": \"string\",\n      \"description\": \"Consumer group\"\n    }\n  },\n  \"required\": [\n    \"receiptHandle\",\n    \"topic\",\n    \"consumerGroup\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-ack-request-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: AckRequest
---
