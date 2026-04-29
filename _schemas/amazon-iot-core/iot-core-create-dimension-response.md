---
description: CreateDimensionResponse schema
layout: schema
name: CreateDimensionResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-dimension-response-schema.json
slug: iot-core-create-dimension-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-dimension-response-schema.json\",\n  \"title\": \"CreateDimensionResponse\",\n  \"description\": \"CreateDimensionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionName\"\n        },\n        {\n          \"description\": \"A unique identifier for the dimension.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DimensionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the created dimension.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-dimension-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateDimensionResponse
---
