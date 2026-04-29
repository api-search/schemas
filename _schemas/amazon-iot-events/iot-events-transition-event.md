---
description: Specifies the actions performed and the next state entered when a <code>condition</code> evaluates to TRUE.
layout: schema
name: TransitionEvent
properties_list:
- description: ''
  name: eventName
  type: object
- description: ''
  name: condition
  type: object
- description: ''
  name: actions
  type: object
- description: ''
  name: nextState
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-transition-event-schema.json
slug: iot-events-transition-event
source_filename: iot-events-transition-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-transition-event-schema.json\",\n  \"title\": \"TransitionEvent\",\n  \"description\": \"Specifies the actions performed and the next state entered when a <code>condition</code> evaluates to TRUE.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventName\"\n        },\n        {\n          \"description\": \"The name of the transition event.\"\n        }\n      ]\n    },\n    \"condition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Condition\"\n        },\n        {\n          \"description\": \"Required. A Boolean expression that when TRUE causes the actions to be performed and the <code>nextState</code> to be entered.\"\n        }\n      ]\n    },\n    \"actions\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Actions\"\n        },\n        {\n          \"description\": \"The actions to be performed.\"\n        }\n      ]\n    },\n    \"nextState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateName\"\n        },\n        {\n          \"description\": \"The next state to enter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"eventName\",\n    \"condition\",\n    \"nextState\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-transition-event-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: TransitionEvent
---
