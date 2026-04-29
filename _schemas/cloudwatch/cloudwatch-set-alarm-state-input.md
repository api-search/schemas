---
description: ''
layout: schema
name: SetAlarmStateInput
properties_list:
- description: The name of the alarm.
  name: AlarmName
  type: string
- description: The reason that this alarm is set to this specific state, in text format.
  name: StateReason
  type: string
- description: The reason that this alarm is set to this specific state, in JSON format.
  name: StateReasonData
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-set-alarm-state-input-schema.json
slug: cloudwatch-set-alarm-state-input
source_filename: cloudwatch-set-alarm-state-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SetAlarmStateInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alarm.\"\n    },\n    \"StateReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason that this alarm is set to this specific state, in text format.\"\n    },\n    \"StateReasonData\": {\n      \"type\": \"string\",\n      \"description\": \"The reason that this alarm is set to this specific state, in JSON format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-set-alarm-state-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: SetAlarmStateInput
---
