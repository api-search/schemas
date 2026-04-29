---
description: ''
layout: schema
name: DescribeAlarmHistoryInput
properties_list:
- description: The name of the alarm.
  name: AlarmName
  type: string
- description: Specify this parameter to receive information only about alarms of the specified types.
  name: AlarmTypes
  type: array
- description: The type of alarm histories to retrieve.
  name: HistoryItemType
  type: string
- description: The starting date to retrieve alarm history.
  name: StartDate
  type: string
- description: The ending date to retrieve alarm history.
  name: EndDate
  type: string
- description: The maximum number of alarm history records to retrieve.
  name: MaxRecords
  type: integer
- description: The token returned by a previous call.
  name: NextToken
  type: string
- description: Specified whether to return the newest or oldest alarm history first.
  name: ScanBy
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarm-history-input-schema.json
slug: cloudwatch-describe-alarm-history-input
source_filename: cloudwatch-describe-alarm-history-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmHistoryInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the alarm.\"\n    },\n    \"AlarmTypes\": {\n      \"type\": \"array\",\n      \"description\": \"Specify this parameter to receive information only about alarms of the specified types.\"\n    },\n    \"HistoryItemType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of alarm histories to retrieve.\"\n    },\n    \"StartDate\": {\n      \"type\": \"string\",\n      \"description\": \"The starting date to retrieve alarm history.\"\n    },\n    \"EndDate\": {\n      \"type\": \"string\",\n      \"description\": \"The ending date to retrieve alarm history.\"\n    },\n    \"MaxRecords\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of alarm history records to retrieve.\"\n    },\n  \
  \  \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token returned by a previous call.\"\n    },\n    \"ScanBy\": {\n      \"type\": \"string\",\n      \"description\": \"Specified whether to return the newest or oldest alarm history first.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarm-history-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmHistoryInput
---
