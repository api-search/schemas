---
description: An auto detection metric source.
layout: schema
name: AutoDetectionMetricSource
properties_list:
- description: ''
  name: S3SourceConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-auto-detection-metric-source-schema.json
slug: amazon-lookout-for-metrics-auto-detection-metric-source
source_filename: amazon-lookout-for-metrics-auto-detection-metric-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-auto-detection-metric-source-schema.json\",\n  \"title\": \"AutoDetectionMetricSource\",\n  \"description\": \"An auto detection metric source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3SourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoDetectionS3SourceConfig\"\n        },\n        {\n          \"description\": \"The source's source config.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-auto-detection-metric-source-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AutoDetectionMetricSource
---
