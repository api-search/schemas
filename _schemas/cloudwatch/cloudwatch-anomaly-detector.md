---
description: An anomaly detection model associated with a particular CloudWatch metric.
layout: schema
name: AnomalyDetector
properties_list:
- description: The namespace of the metric associated with the anomaly detection model.
  name: Namespace
  type: string
- description: The name of the metric associated with the anomaly detection model.
  name: MetricName
  type: string
- description: The metric dimensions associated with the anomaly detection model.
  name: Dimensions
  type: array
- description: The statistic associated with the anomaly detection model.
  name: Stat
  type: string
- description: The current status of the anomaly detector model.
  name: StateValue
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-anomaly-detector-schema.json
slug: cloudwatch-anomaly-detector
source_filename: cloudwatch-anomaly-detector-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnomalyDetector\",\n  \"type\": \"object\",\n  \"description\": \"An anomaly detection model associated with a particular CloudWatch metric.\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric associated with the anomaly detection model.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric associated with the anomaly detection model.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The metric dimensions associated with the anomaly detection model.\"\n    },\n    \"Stat\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic associated with the anomaly detection model.\"\n    },\n    \"StateValue\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the anomaly detector model.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-anomaly-detector-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: AnomalyDetector
---
