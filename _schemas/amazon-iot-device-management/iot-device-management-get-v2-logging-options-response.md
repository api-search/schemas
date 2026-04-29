---
description: GetV2LoggingOptionsResponse schema
layout: schema
name: GetV2LoggingOptionsResponse
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: defaultLogLevel
  type: object
- description: ''
  name: disableAllLogs
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-get-v2-logging-options-response-schema.json
slug: iot-device-management-get-v2-logging-options-response
source_filename: iot-device-management-get-v2-logging-options-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-v2-logging-options-response-schema.json\",\n  \"title\": \"GetV2LoggingOptionsResponse\",\n  \"description\": \"GetV2LoggingOptionsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsArn\"\n        },\n        {\n          \"description\": \"The IAM role ARN IoT uses to write to your CloudWatch logs.\"\n        }\n      ]\n    },\n    \"defaultLogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"The default log level.\"\n        }\n      ]\n    },\n    \"disableAllLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisableAllLogs\"\
  \n        },\n        {\n          \"description\": \"Disables all logs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-get-v2-logging-options-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: GetV2LoggingOptionsResponse
---
