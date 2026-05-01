---
description: The output from the GetLoggingOptions operation.
layout: schema
name: GetLoggingOptionsResponse
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: logLevel
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-get-logging-options-response-schema.json
slug: iot-device-defender-get-logging-options-response
source_filename: iot-device-defender-get-logging-options-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-logging-options-response-schema.json\",\n  \"title\": \"GetLoggingOptionsResponse\",\n  \"description\": \"The output from the GetLoggingOptions operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role that grants access.\"\n        }\n      ]\n    },\n    \"logLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"The logging level.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-get-logging-options-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: GetLoggingOptionsResponse
---
