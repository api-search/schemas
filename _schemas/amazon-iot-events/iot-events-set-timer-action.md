---
description: Information needed to set the timer.
layout: schema
name: SetTimerAction
properties_list:
- description: ''
  name: timerName
  type: object
- description: ''
  name: seconds
  type: object
- description: ''
  name: durationExpression
  type: object
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-set-timer-action-schema.json
slug: iot-events-set-timer-action
source_filename: iot-events-set-timer-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-set-timer-action-schema.json\",\n  \"title\": \"SetTimerAction\",\n  \"description\": \"Information needed to set the timer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerName\"\n        },\n        {\n          \"description\": \"The name of the timer.\"\n        }\n      ]\n    },\n    \"seconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Seconds\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"The number of seconds until the timer expires. The minimum value is 60 seconds to ensure accuracy. The maximum value is 31622400 seconds. seconds is deprecated. You can use durationExpression for SetTimerAction. The value\
  \ of seconds can be used as a string expression for durationExpression.\"\n        }\n      ]\n    },\n    \"durationExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableValue\"\n        },\n        {\n          \"description\": \"The duration of the timer, in seconds. You can use a string expression that includes numbers, variables (<code>$variable.&lt;variable-name&gt;</code>), and input values (<code>$input.&lt;input-name&gt;.&lt;path-to-datum&gt;</code>) as the duration. The range of the duration is 1-31622400 seconds. To ensure accuracy, the minimum duration is 60 seconds. The evaluated result of the duration is rounded down to the nearest whole number. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timerName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-set-timer-action-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: SetTimerAction
---
