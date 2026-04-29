---
description: Specifies one range of days or times to exclude from use for training an anomaly detection model.
layout: schema
name: Range
properties_list:
- description: The start time of the range to exclude.
  name: StartTime
  type: string
- description: The end time of the range to exclude.
  name: EndTime
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-range-schema.json
slug: cloudwatch-range
source_filename: cloudwatch-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Range\",\n  \"type\": \"object\",\n  \"description\": \"Specifies one range of days or times to exclude from use for training an anomaly detection model.\",\n  \"properties\": {\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"description\": \"The start time of the range to exclude.\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"description\": \"The end time of the range to exclude.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-range-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Range
---
