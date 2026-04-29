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
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-create-mitigation-action-response-schema.json
slug: iot-core-create-mitigation-action-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-mitigation-action-response-schema.json\",\n  \"title\": \"CreateMitigationActionResponse\",\n  \"description\": \"CreateMitigationActionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionArn\"\n        },\n        {\n          \"description\": \"The ARN for the new mitigation action.\"\n        }\n      ]\n    },\n    \"actionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MitigationActionId\"\n        },\n        {\n          \"description\": \"A unique identifier for the new mitigation action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-create-mitigation-action-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: CreateMitigationActionResponse
---
