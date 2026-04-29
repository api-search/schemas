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
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-alert-target-schema.json
slug: iot-core-alert-target
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-alert-target-schema.json\",\n  \"title\": \"AlertTarget\",\n  \"description\": \"A structure containing the alert target ARN and the role ARN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alertTargetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertTargetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the notification target to which alerts are sent.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the role that grants permission to send alerts to the notification target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"alertTargetArn\",\n \
  \   \"roleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-alert-target-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: AlertTarget
---
