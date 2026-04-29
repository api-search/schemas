---
description: Information needed to clear the timer.
layout: schema
name: ClearTimerAction
properties_list:
- description: ''
  name: timerName
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-clear-timer-action-schema.json
slug: iot-events-clear-timer-action
source_filename: iot-events-clear-timer-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-clear-timer-action-schema.json\",\n  \"title\": \"ClearTimerAction\",\n  \"description\": \"Information needed to clear the timer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerName\"\n        },\n        {\n          \"description\": \"The name of the timer to clear.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-clear-timer-action-schema.json
tags:
- AWS
- Event Detection
- IoT
- State Machine
- Automation
title: ClearTimerAction
---
