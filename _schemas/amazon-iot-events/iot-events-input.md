---
description: Information about the input.
layout: schema
name: Input
properties_list:
- description: ''
  name: inputConfiguration
  type: object
- description: ''
  name: inputDefinition
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-input-schema.json
slug: iot-events-input
source_filename: iot-events-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"Information about the input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputConfiguration\"\n        },\n        {\n          \"description\": \"Information about the configuration of an input.\"\n        }\n      ]\n    },\n    \"inputDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDefinition\"\n        },\n        {\n          \"description\": \"The definition of the input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: Input
---
