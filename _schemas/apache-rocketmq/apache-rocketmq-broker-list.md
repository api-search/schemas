---
description: List of RocketMQ brokers
layout: schema
name: BrokerList
properties_list:
- description: ''
  name: brokers
  type: array
provider_name: Apache RocketMQ
provider_slug: apache-rocketmq
schema_file: json-schema/apache-rocketmq-broker-list-schema.json
slug: apache-rocketmq-broker-list
source_filename: apache-rocketmq-broker-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-broker-list-schema.json\",\n  \"title\": \"BrokerList\",\n  \"description\": \"List of RocketMQ brokers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brokers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Broker\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-rocketmq/refs/heads/main/json-schema/apache-rocketmq-broker-list-schema.json
tags:
- Cloud Native
- Messaging
- Message Queue
- Pub-Sub
- Streaming
- Apache
- Open Source
title: BrokerList
---
