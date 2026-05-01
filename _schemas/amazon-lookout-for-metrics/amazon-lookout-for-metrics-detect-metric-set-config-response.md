---
description: DetectMetricSetConfigResponse schema from Amazon Lookout for Metrics API
layout: schema
name: DetectMetricSetConfigResponse
properties_list:
- description: ''
  name: DetectedMetricSetConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detect-metric-set-config-response-schema.json
slug: amazon-lookout-for-metrics-detect-metric-set-config-response
source_filename: amazon-lookout-for-metrics-detect-metric-set-config-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detect-metric-set-config-response-schema.json\",\n  \"title\": \"DetectMetricSetConfigResponse\",\n  \"description\": \"DetectMetricSetConfigResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DetectedMetricSetConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedMetricSetConfig\"\n        },\n        {\n          \"description\": \"The inferred dataset configuration for the datasource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detect-metric-set-config-response-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectMetricSetConfigResponse
---
