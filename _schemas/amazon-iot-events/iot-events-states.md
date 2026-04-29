---
description: States schema
layout: schema
name: States
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-states-schema.json
slug: iot-events-states
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-states-schema.json\",\n  \"title\": \"States\",\n  \"description\": \"States schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"stateName\"\n    ],\n    \"properties\": {\n      \"stateName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StateName\"\n          },\n          {\n            \"description\": \"The name of the state.\"\n          }\n        ]\n      },\n      \"onInput\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/OnInputLifecycle\"\n          },\n          {\n            \"description\": \"When an input is received and the <code>condition</code> is TRUE, perform the specified <code>actions</code>.\"\n          }\n        ]\n      },\n      \"onEnter\"\
  : {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/OnEnterLifecycle\"\n          },\n          {\n            \"description\": \"When entering this state, perform these <code>actions</code> if the <code>condition</code> is TRUE.\"\n          }\n        ]\n      },\n      \"onExit\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/OnExitLifecycle\"\n          },\n          {\n            \"description\": \"When exiting this state, perform these <code>actions</code> if the specified <code>condition</code> is <code>TRUE</code>.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Information that defines a state of a detector.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-states-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: States
---
