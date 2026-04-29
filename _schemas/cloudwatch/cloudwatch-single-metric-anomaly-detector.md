---
description: Designates the CloudWatch metric and statistic that provides the time series the anomaly detector uses as input.
layout: schema
name: SingleMetricAnomalyDetector
properties_list:
- description: If the CloudWatch metric that provides the time series is in another account, use this to specify that account ID.
  name: AccountId
  type: string
- description: The namespace of the metric to create the anomaly detection model for.
  name: Namespace
  type: string
- description: The name of the metric to create the anomaly detection model for.
  name: MetricName
  type: string
- description: The metric dimensions to create the anomaly detection model for.
  name: Dimensions
  type: array
- description: The statistic to use for the metric and anomaly detection model.
  name: Stat
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-single-metric-anomaly-detector-schema.json
slug: cloudwatch-single-metric-anomaly-detector
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SingleMetricAnomalyDetector\",\n  \"type\": \"object\",\n  \"description\": \"Designates the CloudWatch metric and statistic that provides the time series the anomaly detector uses as input.\",\n  \"properties\": {\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"If the CloudWatch metric that provides the time series is in another account, use this to specify that account ID.\"\n    },\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric to create the anomaly detection model for.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric to create the anomaly detection model for.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The metric dimensions to create the anomaly detection model for.\"\n    },\n    \"Stat\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The statistic to use for the metric and anomaly detection model.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-single-metric-anomaly-detector-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: SingleMetricAnomalyDetector
---
