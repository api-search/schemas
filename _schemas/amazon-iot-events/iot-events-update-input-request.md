---
description: UpdateInputRequest schema
layout: schema
name: UpdateInputRequest
properties_list:
- description: ''
  name: inputDescription
  type: object
- description: ''
  name: inputDefinition
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-update-input-request-schema.json
slug: iot-events-update-input-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-input-request-schema.json\",\n  \"title\": \"UpdateInputRequest\",\n  \"description\": \"UpdateInputRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDescription\"\n        },\n        {\n          \"description\": \"A brief description of the input.\"\n        }\n      ]\n    },\n    \"inputDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDefinition\"\n        },\n        {\n          \"description\": \"The definition of the input.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-input-request-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: UpdateInputRequest
---
