---
description: CreateMitigationActionResponse schema
layout: schema
name: CreateMitigationActionResponse
properties_list:
- description: ''
  name: actionArn
  type: object
- description: ''
  name: actionId
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-mitigation-action-response-schema.json
slug: iot-device-defender-create-mitigation-action-response
source_filename: iot-device-defender-create-mitigation-action-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-mitigation-action-response-schema.json\",\n  \"title\": \"CreateMitigationActionResponse\",\n  \"description\": \"CreateMitigationActionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionArn\"\n        },\n        {\n          \"description\": \"The ARN for the new mitigation action.\"\n        }\n      ]\n    },\n    \"actionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionId\"\n        },\n        {\n          \"description\": \"A unique identifier for the new mitigation action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-mitigation-action-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateMitigationActionResponse
---
