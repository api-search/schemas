---
description: Types of broker engines.
layout: schema
name: BrokerEngineType
properties_list:
- description: ''
  name: EngineType
  type: object
- description: ''
  name: EngineVersions
  type: object
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-broker-engine-type-schema.json
slug: mq-api-broker-engine-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-engine-type-schema.json\",\n  \"title\": \"BrokerEngineType\",\n  \"description\": \"Types of broker engines.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineType\"\n          },\n          \"description\": \"The broker's engine type.\"\n        }\n      ]\n    },\n    \"EngineVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfEngineVersion\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"engineVersions\"\n          },\n          \"description\": \"The list of engine versions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-broker-engine-type-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerEngineType
---
