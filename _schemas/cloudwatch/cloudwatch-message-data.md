---
description: A message returned by the GetMetricData API.
layout: schema
name: MessageData
properties_list:
- description: The error code or status code associated with the message.
  name: Code
  type: string
- description: The message text.
  name: Value
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-message-data-schema.json
slug: cloudwatch-message-data
source_filename: cloudwatch-message-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageData\",\n  \"type\": \"object\",\n  \"description\": \"A message returned by the GetMetricData API.\",\n  \"properties\": {\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code or status code associated with the message.\"\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The message text.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-message-data-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MessageData
---
