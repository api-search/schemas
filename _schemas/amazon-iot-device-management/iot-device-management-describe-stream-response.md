---
description: DescribeStreamResponse schema
layout: schema
name: DescribeStreamResponse
properties_list:
- description: ''
  name: streamInfo
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-stream-response-schema.json
slug: iot-device-management-describe-stream-response
source_filename: iot-device-management-describe-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-stream-response-schema.json\",\n  \"title\": \"DescribeStreamResponse\",\n  \"description\": \"DescribeStreamResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamInfo\"\n        },\n        {\n          \"description\": \"Information about the stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-stream-response-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeStreamResponse
---
