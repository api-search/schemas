---
description: Specifies the actions performed when the <code>condition</code> evaluates to TRUE.
layout: schema
name: OnInputLifecycle
properties_list:
- description: ''
  name: events
  type: object
- description: ''
  name: transitionEvents
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-on-input-lifecycle-schema.json
slug: iot-events-on-input-lifecycle
source_filename: iot-events-on-input-lifecycle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-on-input-lifecycle-schema.json\",\n  \"title\": \"OnInputLifecycle\",\n  \"description\": \"Specifies the actions performed when the <code>condition</code> evaluates to TRUE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Events\"\n        },\n        {\n          \"description\": \"Specifies the actions performed when the <code>condition</code> evaluates to TRUE.\"\n        }\n      ]\n    },\n    \"transitionEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransitionEvents\"\n        },\n        {\n          \"description\": \"Specifies the actions performed, and the next state entered, when a <code>condition</code> evaluates to TRUE.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-on-input-lifecycle-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: OnInputLifecycle
---
