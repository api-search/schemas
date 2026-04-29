---
description: Request to create a RocketMQ topic
layout: schema
name: TopicRequest
properties_list:
- description: Topic name
  name: name
  type: string
- description: Target cluster
  name: clusterName
  type: string
- description: Number of queues (default 8)
  name: queueNum
  type: integer
- description: Permission (6 = read+write)
  name: perm
  type: integer
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-topic-request-schema.json
slug: apache-rocketmq-topic-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-request-schema.json\",\n  \"title\": \"TopicRequest\",\n  \"description\": \"Request to create a RocketMQ topic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Topic name\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Target cluster\"\n    },\n    \"queueNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of queues (default 8)\"\n    },\n    \"perm\": {\n      \"type\": \"integer\",\n      \"description\": \"Permission (6 = read+write)\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-request-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: TopicRequest
---
