---
description: Represents the history of a specific alarm.
layout: schema
name: AlarmHistoryItem
properties_list:
- description: The descriptive name for the alarm.
  name: AlarmName
  type: string
- description: The type of alarm, either metric alarm or composite alarm.
  name: AlarmType
  type: string
- description: The time stamp for the alarm history item.
  name: Timestamp
  type: string
- description: The type of alarm history item.
  name: HistoryItemType
  type: string
- description: A summary of the alarm history, in text format.
  name: HistorySummary
  type: string
- description: Data about the alarm, in JSON format.
  name: HistoryData
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-alarm-history-item-schema.json
slug: cloudwatch-alarm-history-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlarmHistoryItem\",\n  \"type\": \"object\",\n  \"description\": \"Represents the history of a specific alarm.\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The descriptive name for the alarm.\"\n    },\n    \"AlarmType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of alarm, either metric alarm or composite alarm.\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp for the alarm history item.\"\n    },\n    \"HistoryItemType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of alarm history item.\"\n    },\n    \"HistorySummary\": {\n      \"type\": \"string\",\n      \"description\": \"A summary of the alarm history, in text format.\"\n    },\n    \"HistoryData\": {\n      \"type\": \"string\",\n      \"description\": \"Data about the alarm, in JSON\
  \ format.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-alarm-history-item-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: AlarmHistoryItem
---
