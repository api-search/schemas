---
description: The definition of the input.
layout: schema
name: InputDefinition
properties_list:
- description: ''
  name: attributes
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-input-definition-schema.json
slug: iot-events-input-definition
source_filename: iot-events-input-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-definition-schema.json\",\n  \"title\": \"InputDefinition\",\n  \"description\": \"The definition of the input.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Attributes\"\n        },\n        {\n          \"description\": \"The attributes from the JSON payload that are made available by the input. Inputs are derived from messages sent to the AWS IoT Events system using <code>BatchPutMessage</code>. Each such message contains a JSON payload, and those attributes (and their paired values) specified here are available for use in the <code>condition</code> expressions used by detectors that monitor this input. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"attributes\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-input-definition-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: InputDefinition
---
