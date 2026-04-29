---
description: CreateBrokerResponse schema from Amazon MQ API
layout: schema
name: CreateBrokerResponse
properties_list:
- description: ''
  name: BrokerArn
  type: object
- description: ''
  name: BrokerId
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-create-broker-response-schema.json
slug: mq-api-create-broker-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-broker-response-schema.json\",\n  \"title\": \"CreateBrokerResponse\",\n  \"description\": \"CreateBrokerResponse schema from Amazon MQ API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BrokerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerArn\"\n          },\n          \"description\": \"The broker's Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"BrokerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"brokerId\"\n          },\n          \"description\": \"The unique ID that Amazon MQ generates for the broker.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-create-broker-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateBrokerResponse
---
