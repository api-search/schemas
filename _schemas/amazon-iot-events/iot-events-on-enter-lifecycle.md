---
description: When entering this state, perform these <code>actions</code> if the <code>condition</code> is TRUE.
layout: schema
name: OnEnterLifecycle
properties_list:
- description: ''
  name: events
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-on-enter-lifecycle-schema.json
slug: iot-events-on-enter-lifecycle
source_filename: iot-events-on-enter-lifecycle-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-on-enter-lifecycle-schema.json\",\n  \"title\": \"OnEnterLifecycle\",\n  \"description\": \"When entering this state, perform these <code>actions</code> if the <code>condition</code> is TRUE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Events\"\n        },\n        {\n          \"description\": \"Specifies the actions that are performed when the state is entered and the <code>condition</code> is <code>TRUE</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-on-enter-lifecycle-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: OnEnterLifecycle
---
