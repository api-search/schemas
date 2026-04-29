---
description: Information about the variable and its new value.
layout: schema
name: SetVariableAction
properties_list:
- description: ''
  name: variableName
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-set-variable-action-schema.json
slug: iot-events-set-variable-action
source_filename: iot-events-set-variable-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-set-variable-action-schema.json\",\n  \"title\": \"SetVariableAction\",\n  \"description\": \"Information about the variable and its new value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"variableName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableName\"\n        },\n        {\n          \"description\": \"The name of the variable.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableValue\"\n        },\n        {\n          \"description\": \"The new value of the variable.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"variableName\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-set-variable-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: SetVariableAction
---
