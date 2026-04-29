---
description: RocketMQ broker
layout: schema
name: Broker
properties_list:
- description: Broker name
  name: brokerName
  type: string
- description: Cluster identifier
  name: clusterId
  type: string
- description: Broker ID (0=master, >0=slave)
  name: brokerId
  type: integer
- description: Broker address (host:port)
  name: brokerAddr
  type: string
- description: Broker version
  name: version
  type: string
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-broker-schema.json
slug: apache-rocketmq-broker
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-broker-schema.json\",\n  \"title\": \"Broker\",\n  \"description\": \"RocketMQ broker\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brokerName\": {\n      \"type\": \"string\",\n      \"description\": \"Broker name\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster identifier\"\n    },\n    \"brokerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Broker ID (0=master, >0=slave)\"\n    },\n    \"brokerAddr\": {\n      \"type\": \"string\",\n      \"description\": \"Broker address (host:port)\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Broker version\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-broker-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: Broker
---
