---
description: The configuration specifies details about how the anomaly detection model is to be trained.
layout: schema
name: AnomalyDetectorConfiguration
properties_list:
- description: An array of time ranges to exclude from use when the anomaly detection model is trained.
  name: ExcludedTimeRanges
  type: array
- description: The time zone to use for the metric.
  name: MetricTimezone
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-anomaly-detector-configuration-schema.json
slug: cloudwatch-anomaly-detector-configuration
source_filename: cloudwatch-anomaly-detector-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AnomalyDetectorConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"The configuration specifies details about how the anomaly detection model is to be trained.\",\n  \"properties\": {\n    \"ExcludedTimeRanges\": {\n      \"type\": \"array\",\n      \"description\": \"An array of time ranges to exclude from use when the anomaly detection model is trained.\"\n    },\n    \"MetricTimezone\": {\n      \"type\": \"string\",\n      \"description\": \"The time zone to use for the metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-anomaly-detector-configuration-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: AnomalyDetectorConfiguration
---
