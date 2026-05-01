---
description: Returns information about all brokers.
layout: schema
name: BrokerInstance
properties_list:
- description: ''
  name: ConsoleURL
  type: object
- description: ''
  name: Endpoints
  type: object
- description: ''
  name: IpAddress
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-instance-schema.json
slug: mq-api-broker-instance
source_filename: mq-api-broker-instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-instance-schema.json\",\n  \"title\": \"BrokerInstance\",\n  \"description\": \"Returns information about all brokers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConsoleURL\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"consoleURL\"\n          },\n          \"description\": \"The brokers web console URL.\"\n        }\n      ]\n    },\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endpoints\"\n          },\n          \"description\": \"The broker's wire-level protocol endpoints.\"\n        }\n      ]\n    },\n    \"IpAddress\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ipAddress\"\n          },\n          \"description\": \"The IP address of the Elastic Network Interface (ENI) attached to the broker. Does not apply to RabbitMQ brokers.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-instance-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: BrokerInstance
---
