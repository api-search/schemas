---
description: CreateInputRequest schema
layout: schema
name: CreateInputRequest
properties_list:
- description: ''
  name: inputName
  type: object
- description: ''
  name: inputDescription
  type: object
- description: ''
  name: inputDefinition
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-create-input-request-schema.json
slug: iot-events-create-input-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-input-request-schema.json\",\n  \"title\": \"CreateInputRequest\",\n  \"description\": \"CreateInputRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputName\"\n        },\n        {\n          \"description\": \"The name you want to give to the input.\"\n        }\n      ]\n    },\n    \"inputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDescription\"\n        },\n        {\n          \"description\": \"A brief description of the input.\"\n        }\n      ]\n    },\n    \"inputDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDefinition\"\n        },\n        {\n          \"\
  description\": \"The definition of the input.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"Metadata that can be used to manage the input.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputName\",\n    \"inputDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-create-input-request-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: CreateInputRequest
---
