---
description: DescribeStreamResponse schema
layout: schema
name: DescribeStreamResponse
properties_list:
- description: ''
  name: streamInfo
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-stream-response-schema.json
slug: iot-device-defender-describe-stream-response
source_filename: iot-device-defender-describe-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-stream-response-schema.json\",\n  \"title\": \"DescribeStreamResponse\",\n  \"description\": \"DescribeStreamResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamInfo\"\n        },\n        {\n          \"description\": \"Information about the stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-stream-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeStreamResponse
---
