---
description: ''
layout: schema
name: GetMetricDataOutput
properties_list:
- description: The metrics that are returned, including the metric name, namespace, and dimensions.
  name: MetricDataResults
  type: array
- description: A token that marks the next batch of returned results.
  name: NextToken
  type: string
- description: Contains a message about the operation or the results.
  name: Messages
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-metric-data-output-schema.json
slug: cloudwatch-get-metric-data-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMetricDataOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricDataResults\": {\n      \"type\": \"array\",\n      \"description\": \"The metrics that are returned, including the metric name, namespace, and dimensions.\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\",\n      \"description\": \"A token that marks the next batch of returned results.\"\n    },\n    \"Messages\": {\n      \"type\": \"array\",\n      \"description\": \"Contains a message about the operation or the results.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-data-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetMetricDataOutput
---
