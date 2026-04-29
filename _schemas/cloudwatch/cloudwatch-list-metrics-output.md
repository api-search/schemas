---
description: ''
layout: schema
name: ListMetricsOutput
properties_list:
- description: The metrics that match your request.
  name: Metrics
  type: array
- description: The token that marks the start of the next batch of returned results.
  name: NextToken
  type: string
- description: If you are using this operation in a monitoring account, this array contains the account IDs of the source accounts.
  name: OwningAccounts
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-list-metrics-output-schema.json
slug: cloudwatch-list-metrics-output
source_filename: cloudwatch-list-metrics-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListMetricsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Metrics\": {\n      \"type\": \"array\",\n      \"description\": \"The metrics that match your request.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"The token that marks the start of the next batch of returned results.\"\n    },\n    \"OwningAccounts\": {\n      \"type\": \"array\",\n      \"description\": \"If you are using this operation in a monitoring account, this array contains the account IDs of the source accounts.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-list-metrics-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: ListMetricsOutput
---
