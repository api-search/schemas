---
description: ''
layout: schema
name: PutMetricDataInput
properties_list:
- description: The namespace for the metric data. To avoid conflicts with AWS service namespaces, you should not specify a namespace that begins with AWS/.
  name: Namespace
  type: string
- description: The data for the metric. The array can include no more than 1000 metrics per call.
  name: MetricData
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-metric-data-input-schema.json
slug: cloudwatch-put-metric-data-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutMetricDataInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace for the metric data. To avoid conflicts with AWS service namespaces, you should not specify a namespace that begins with AWS/.\"\n    },\n    \"MetricData\": {\n      \"type\": \"array\",\n      \"description\": \"The data for the metric. The array can include no more than 1000 metrics per call.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-metric-data-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutMetricDataInput
---
