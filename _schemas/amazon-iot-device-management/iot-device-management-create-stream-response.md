---
description: CreateStreamResponse schema
layout: schema
name: CreateStreamResponse
properties_list:
- description: ''
  name: streamId
  type: object
- description: ''
  name: streamArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: streamVersion
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-create-stream-response-schema.json
slug: iot-device-management-create-stream-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-stream-response-schema.json\",\n  \"title\": \"CreateStreamResponse\",\n  \"description\": \"CreateStreamResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamId\"\n        },\n        {\n          \"description\": \"The stream ID.\"\n        }\n      ]\n    },\n    \"streamArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamArn\"\n        },\n        {\n          \"description\": \"The stream ARN.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamDescription\"\n        },\n        {\n          \"description\": \"A description of\
  \ the stream.\"\n        }\n      ]\n    },\n    \"streamVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamVersion\"\n        },\n        {\n          \"description\": \"The version of the stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-create-stream-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: CreateStreamResponse
---
