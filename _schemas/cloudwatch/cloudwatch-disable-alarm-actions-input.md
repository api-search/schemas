---
description: ''
layout: schema
name: DisableAlarmActionsInput
properties_list:
- description: The names of the alarms.
  name: AlarmNames
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-disable-alarm-actions-input-schema.json
slug: cloudwatch-disable-alarm-actions-input
source_filename: cloudwatch-disable-alarm-actions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DisableAlarmActionsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmNames\": {\n      \"type\": \"array\",\n      \"description\": \"The names of the alarms.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-disable-alarm-actions-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DisableAlarmActionsInput
---
