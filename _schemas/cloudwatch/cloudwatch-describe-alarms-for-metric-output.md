---
description: ''
layout: schema
name: DescribeAlarmsForMetricOutput
properties_list:
- description: The information for each alarm with the specified metric.
  name: MetricAlarms
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarms-for-metric-output-schema.json
slug: cloudwatch-describe-alarms-for-metric-output
source_filename: cloudwatch-describe-alarms-for-metric-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmsForMetricOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricAlarms\": {\n      \"type\": \"array\",\n      \"description\": \"The information for each alarm with the specified metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-for-metric-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmsForMetricOutput
---
