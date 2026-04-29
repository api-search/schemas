---
description: ''
layout: schema
name: ListMetricStreamsOutput
properties_list:
- description: The array of metric stream information.
  name: Entries
  type: array
- description: The token that marks the start of the next batch of returned results.
  name: NextToken
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-metric-streams-output-schema.json
slug: cloudwatch-list-metric-streams-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMetricStreamsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entries\": {\n      \"type\": \"array\",\n      \"description\": \"The array of metric stream information.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token that marks the start of the next batch of returned results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-metric-streams-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListMetricStreamsOutput
---
