---
description: Events schema
layout: schema
name: Events
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-events-schema.json
slug: iot-events-events
source_filename: iot-events-events-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-events-schema.json\",\n  \"title\": \"Events\",\n  \"description\": \"Events schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"required\": [\n      \"eventName\"\n    ],\n    \"properties\": {\n      \"eventName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/EventName\"\n          },\n          {\n            \"description\": \"The name of the event.\"\n          }\n        ]\n      },\n      \"condition\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Condition\"\n          },\n          {\n            \"description\": \"Optional. The Boolean expression that, when TRUE, causes the <code>actions</code> to be performed. If not present, the actions are performed (=TRUE). If the expression\
  \ result is not a Boolean value, the actions are not performed (=FALSE).\"\n          }\n        ]\n      },\n      \"actions\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Actions\"\n          },\n          {\n            \"description\": \"The actions to be performed.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Specifies the <code>actions</code> to be performed when the <code>condition</code> evaluates to TRUE.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-events-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: Events
---
