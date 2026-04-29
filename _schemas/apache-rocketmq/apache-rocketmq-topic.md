---
description: RocketMQ topic
layout: schema
name: Topic
properties_list:
- description: Topic name
  name: name
  type: string
- description: Cluster name
  name: clusterName
  type: string
- description: Number of message queues
  name: queueNum
  type: integer
- description: Permission flags (2=write, 4=read, 6=read+write)
  name: perm
  type: integer
- description: ''
  name: topicFilterType
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-topic-schema.json
slug: apache-rocketmq-topic
source_filename: apache-rocketmq-topic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-schema.json\",\n  \"title\": \"Topic\",\n  \"description\": \"RocketMQ topic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Topic name\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster name\"\n    },\n    \"queueNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of message queues\"\n    },\n    \"perm\": {\n      \"type\": \"integer\",\n      \"description\": \"Permission flags (2=write, 4=read, 6=read+write)\"\n    },\n    \"topicFilterType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SINGLE_TAG\",\n        \"MULTI_TAG\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-topic-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Topic
---
