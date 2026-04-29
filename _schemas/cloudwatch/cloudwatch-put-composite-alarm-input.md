---
description: ''
layout: schema
name: PutCompositeAlarmInput
properties_list:
- description: The name for the composite alarm.
  name: AlarmName
  type: string
- description: The description for the composite alarm.
  name: AlarmDescription
  type: string
- description: Indicates whether actions should be executed during any changes to the alarm state.
  name: ActionsEnabled
  type: boolean
- description: The actions to execute when this alarm transitions to the ALARM state.
  name: AlarmActions
  type: array
- description: An expression that specifies which other alarms are to be evaluated to determine this composite alarm's state.
  name: AlarmRule
  type: string
- description: The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state.
  name: InsufficientDataActions
  type: array
- description: The actions to execute when this alarm transitions to the OK state.
  name: OKActions
  type: array
- description: A list of key-value pairs to associate with the composite alarm.
  name: Tags
  type: array
- description: Actions will be suppressed if the suppressor alarm is in the ALARM state.
  name: ActionsSuppressor
  type: string
- description: The maximum time in seconds that the composite alarm waits for the suppressor to go into ALARM state.
  name: ActionsSuppressorWaitPeriod
  type: integer
- description: The maximum time in seconds that the composite alarm waits after the suppressor leaves the ALARM state.
  name: ActionsSuppressorExtensionPeriod
  type: integer
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-composite-alarm-input-schema.json
slug: cloudwatch-put-composite-alarm-input
source_filename: cloudwatch-put-composite-alarm-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutCompositeAlarmInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the composite alarm.\"\n    },\n    \"AlarmDescription\": {\n      \"type\": \"string\",\n      \"description\": \"The description for the composite alarm.\"\n    },\n    \"ActionsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether actions should be executed during any changes to the alarm state.\"\n    },\n    \"AlarmActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the ALARM state.\"\n    },\n    \"AlarmRule\": {\n      \"type\": \"string\",\n      \"description\": \"An expression that specifies which other alarms are to be evaluated to determine this composite alarm's state.\"\n    },\n    \"InsufficientDataActions\": {\n   \
  \   \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the INSUFFICIENT_DATA state.\"\n    },\n    \"OKActions\": {\n      \"type\": \"array\",\n      \"description\": \"The actions to execute when this alarm transitions to the OK state.\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"description\": \"A list of key-value pairs to associate with the composite alarm.\"\n    },\n    \"ActionsSuppressor\": {\n      \"type\": \"string\",\n      \"description\": \"Actions will be suppressed if the suppressor alarm is in the ALARM state.\"\n    },\n    \"ActionsSuppressorWaitPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum time in seconds that the composite alarm waits for the suppressor to go into ALARM state.\"\n    },\n    \"ActionsSuppressorExtensionPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum time in seconds that the composite alarm waits after the suppressor\
  \ leaves the ALARM state.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-composite-alarm-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutCompositeAlarmInput
---
