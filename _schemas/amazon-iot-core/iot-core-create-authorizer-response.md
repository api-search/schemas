---
description: CreateAuthorizerResponse schema
layout: schema
name: CreateAuthorizerResponse
properties_list:
- description: ''
  name: authorizerName
  type: object
- description: ''
  name: authorizerArn
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-authorizer-response-schema.json
slug: iot-core-create-authorizer-response
source_filename: iot-core-create-authorizer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-authorizer-response-schema.json\",\n  \"title\": \"CreateAuthorizerResponse\",\n  \"description\": \"CreateAuthorizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerName\"\n        },\n        {\n          \"description\": \"The authorizer's name.\"\n        }\n      ]\n    },\n    \"authorizerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerArn\"\n        },\n        {\n          \"description\": \"The authorizer ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-authorizer-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateAuthorizerResponse
---
