---
description: GetDataQualityMetricsResponse schema from Amazon Lookout for Metrics API
layout: schema
name: GetDataQualityMetricsResponse
properties_list:
- description: ''
  name: AnomalyDetectorDataQualityMetricList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-response-schema.json
slug: amazon-lookout-for-metrics-get-data-quality-metrics-response
source_filename: amazon-lookout-for-metrics-get-data-quality-metrics-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-response-schema.json\",\n  \"title\": \"GetDataQualityMetricsResponse\",\n  \"description\": \"GetDataQualityMetricsResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorDataQualityMetricList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorDataQualityMetricList\"\n        },\n        {\n          \"description\": \"A list of the data quality metrics for the <code>AnomalyDetectorArn</code> that you requested.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-data-quality-metrics-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetDataQualityMetricsResponse
---
