---
description: An inferred dataset configuration.
layout: schema
name: DetectedMetricSetConfig
properties_list:
- description: ''
  name: Offset
  type: object
- description: ''
  name: MetricSetFrequency
  type: object
- description: ''
  name: MetricSource
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-metric-set-config-schema.json
slug: amazon-lookout-for-metrics-detected-metric-set-config
source_filename: amazon-lookout-for-metrics-detected-metric-set-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-metric-set-config-schema.json\",\n  \"title\": \"DetectedMetricSetConfig\",\n  \"description\": \"An inferred dataset configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Offset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The dataset's offset.\"\n        }\n      ]\n    },\n    \"MetricSetFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedField\"\n        },\n        {\n          \"description\": \"The dataset's interval.\"\n        }\n      ]\n    },\n    \"MetricSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedMetricSource\"\n        },\n   \
  \     {\n          \"description\": \"The dataset's data source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-metric-set-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedMetricSetConfig
---
