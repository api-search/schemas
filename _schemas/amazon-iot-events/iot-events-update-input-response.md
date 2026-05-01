---
description: UpdateInputResponse schema
layout: schema
name: UpdateInputResponse
properties_list:
- description: ''
  name: inputConfiguration
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-update-input-response-schema.json
slug: iot-events-update-input-response
source_filename: iot-events-update-input-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-input-response-schema.json\",\n  \"title\": \"UpdateInputResponse\",\n  \"description\": \"UpdateInputResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputConfiguration\"\n        },\n        {\n          \"description\": \"Information about the configuration of the input.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-update-input-response-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: UpdateInputResponse
---
