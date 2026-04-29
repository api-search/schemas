---
description: Indicates the CloudWatch math expression that provides the time series the anomaly detector uses as input.
layout: schema
name: MetricMathAnomalyDetector
properties_list:
- description: An array of metric data query structures that enables you to create an anomaly detector based on the result of a metric math expression.
  name: MetricDataQueries
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-math-anomaly-detector-schema.json
slug: cloudwatch-metric-math-anomaly-detector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricMathAnomalyDetector\",\n  \"type\": \"object\",\n  \"description\": \"Indicates the CloudWatch math expression that provides the time series the anomaly detector uses as input.\",\n  \"properties\": {\n    \"MetricDataQueries\": {\n      \"type\": \"array\",\n      \"description\": \"An array of metric data query structures that enables you to create an anomaly detector based on the result of a metric math expression.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-math-anomaly-detector-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricMathAnomalyDetector
---
