---
description: ''
layout: schema
name: ListDashboardsOutput
properties_list:
- description: The list of matching dashboards.
  name: DashboardEntries
  type: array
- description: The token that marks the start of the next batch of returned results.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-dashboards-output-schema.json
slug: cloudwatch-list-dashboards-output
source_filename: cloudwatch-list-dashboards-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListDashboardsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DashboardEntries\": {\n      \"type\": \"array\",\n      \"description\": \"The list of matching dashboards.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token that marks the start of the next batch of returned results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-dashboards-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListDashboardsOutput
---
