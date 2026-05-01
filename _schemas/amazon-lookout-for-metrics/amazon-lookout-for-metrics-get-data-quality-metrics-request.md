---
description: GetDataQualityMetricsRequest schema from Amazon Lookout for Metrics API
layout: schema
name: GetDataQualityMetricsRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: MetricSetArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-request-schema.json
slug: amazon-lookout-for-metrics-get-data-quality-metrics-request
source_filename: amazon-lookout-for-metrics-get-data-quality-metrics-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-request-schema.json\",\n  \"title\": \"GetDataQualityMetricsRequest\",\n  \"description\": \"GetDataQualityMetricsRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the anomaly detector that you want to investigate.\"\n        }\n      ]\n    },\n    \"MetricSetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of a specific data quality metric set.\"\n        }\n      ]\n   \
  \ }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetDataQualityMetricsRequest
---
