---
description: A structure containing the alert target ARN and the role ARN.
layout: schema
name: AlertTarget
properties_list:
- description: ''
  name: alertTargetArn
  type: object
- description: ''
  name: roleArn
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-alert-target-schema.json
slug: iot-device-management-alert-target
source_filename: iot-device-management-alert-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-alert-target-schema.json\",\n  \"title\": \"AlertTarget\",\n  \"description\": \"A structure containing the alert target ARN and the role ARN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alertTargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertTargetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the notification target to which alerts are sent.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to send alerts to the notification target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"alertTargetArn\",\n    \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-alert-target-schema.json
tags:
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: AlertTarget
---
