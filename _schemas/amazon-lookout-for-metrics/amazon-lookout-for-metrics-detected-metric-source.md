---
description: An inferred data source.
layout: schema
name: DetectedMetricSource
properties_list:
- description: ''
  name: S3SourceConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-metric-source-schema.json
slug: amazon-lookout-for-metrics-detected-metric-source
source_filename: amazon-lookout-for-metrics-detected-metric-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-metric-source-schema.json\",\n  \"title\": \"DetectedMetricSource\",\n  \"description\": \"An inferred data source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3SourceConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedS3SourceConfig\"\n        },\n        {\n          \"description\": \"The data source's source configuration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-metric-source-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedMetricSource
---
