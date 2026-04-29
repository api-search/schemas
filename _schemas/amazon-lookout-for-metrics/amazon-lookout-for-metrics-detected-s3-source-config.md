---
description: An inferred source configuration.
layout: schema
name: DetectedS3SourceConfig
properties_list:
- description: ''
  name: FileFormatDescriptor
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detected-s3-source-config-schema.json
slug: amazon-lookout-for-metrics-detected-s3-source-config
source_filename: amazon-lookout-for-metrics-detected-s3-source-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-s3-source-config-schema.json\",\n  \"title\": \"DetectedS3SourceConfig\",\n  \"description\": \"An inferred source configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileFormatDescriptor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DetectedFileFormatDescriptor\"\n        },\n        {\n          \"description\": \"The source's file format descriptor.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detected-s3-source-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectedS3SourceConfig
---
