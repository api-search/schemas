---
description: ''
layout: schema
name: DeleteAlarmsInput
properties_list:
- description: The alarms to be deleted. You can delete up to 100 alarms in one operation.
  name: AlarmNames
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-delete-alarms-input-schema.json
slug: cloudwatch-delete-alarms-input
source_filename: cloudwatch-delete-alarms-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteAlarmsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlarmNames\": {\n      \"type\": \"array\",\n      \"description\": \"The alarms to be deleted. You can delete up to 100 alarms in one operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-delete-alarms-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DeleteAlarmsInput
---
