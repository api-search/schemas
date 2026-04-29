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
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-authorizer-response-schema.json
slug: iot-device-management-create-authorizer-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-authorizer-response-schema.json\",\n  \"title\": \"CreateAuthorizerResponse\",\n  \"description\": \"CreateAuthorizerResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerName\"\n        },\n        {\n          \"description\": \"The authorizer's name.\"\n        }\n      ]\n    },\n    \"authorizerArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizerArn\"\n        },\n        {\n          \"description\": \"The authorizer ARN.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-authorizer-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateAuthorizerResponse
---
