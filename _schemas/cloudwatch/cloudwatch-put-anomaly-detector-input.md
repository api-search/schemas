---
description: ''
layout: schema
name: PutAnomalyDetectorInput
properties_list:
- description: The namespace of the metric to create the anomaly detection model for.
  name: Namespace
  type: string
- description: The name of the metric to create the anomaly detection model for.
  name: MetricName
  type: string
- description: The metric dimensions to create the anomaly detection model for.
  name: Dimensions
  type: array
- description: The statistic to use for the metric and the anomaly detection model.
  name: Stat
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-put-anomaly-detector-input-schema.json
slug: cloudwatch-put-anomaly-detector-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PutAnomalyDetectorInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric to create the anomaly detection model for.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric to create the anomaly detection model for.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The metric dimensions to create the anomaly detection model for.\"\n    },\n    \"Stat\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic to use for the metric and the anomaly detection model.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-put-anomaly-detector-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: PutAnomalyDetectorInput
---
