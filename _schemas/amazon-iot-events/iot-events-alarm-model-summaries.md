---
description: AlarmModelSummaries schema
layout: schema
name: AlarmModelSummaries
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-model-summaries-schema.json
slug: iot-events-alarm-model-summaries
source_filename: iot-events-alarm-model-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-model-summaries-schema.json\",\n  \"title\": \"AlarmModelSummaries\",\n  \"description\": \"AlarmModelSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time the alarm model was created, in the Unix epoch format.\"\n          }\n        ]\n      },\n      \"alarmModelDescription\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelDescription\"\n          },\n          {\n            \"description\": \"The description of the alarm model.\"\n          }\n        ]\n      },\n      \"alarmModelName\": {\n\
  \        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelName\"\n          },\n          {\n            \"description\": \"The name of the alarm model.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a summary of an alarm model.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-model-summaries-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmModelSummaries
---
