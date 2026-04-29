---
description: ''
layout: schema
name: ListMetricStreamsInput
properties_list:
- description: Include this value to get the next set of metric streams.
  name: NextToken
  type: string
- description: The maximum number of results to return in one operation.
  name: MaxResults
  type: integer
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-metric-streams-input-schema.json
slug: cloudwatch-list-metric-streams-input
source_filename: cloudwatch-list-metric-streams-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMetricStreamsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Include this value to get the next set of metric streams.\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results to return in one operation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-metric-streams-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListMetricStreamsInput
---
