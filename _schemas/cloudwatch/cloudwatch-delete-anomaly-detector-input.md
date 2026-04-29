---
description: ''
layout: schema
name: DeleteAnomalyDetectorInput
properties_list:
- description: The namespace associated with the anomaly detection model to delete.
  name: Namespace
  type: string
- description: The metric name associated with the anomaly detection model to delete.
  name: MetricName
  type: string
- description: The metric dimensions associated with the anomaly detection model to delete.
  name: Dimensions
  type: array
- description: The statistic associated with the anomaly detection model to delete.
  name: Stat
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-delete-anomaly-detector-input-schema.json
slug: cloudwatch-delete-anomaly-detector-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteAnomalyDetectorInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace associated with the anomaly detection model to delete.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The metric name associated with the anomaly detection model to delete.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The metric dimensions associated with the anomaly detection model to delete.\"\n    },\n    \"Stat\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic associated with the anomaly detection model to delete.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-delete-anomaly-detector-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DeleteAnomalyDetectorInput
---
