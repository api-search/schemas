---
description: An auto detection source config.
layout: schema
name: AutoDetectionS3SourceConfig
properties_list:
- description: ''
  name: TemplatedPathList
  type: object
- description: ''
  name: HistoricalDataPathList
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-auto-detection-s3-source-config-schema.json
slug: amazon-lookout-for-metrics-auto-detection-s3-source-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-auto-detection-s3-source-config-schema.json\",\n  \"title\": \"AutoDetectionS3SourceConfig\",\n  \"description\": \"An auto detection source config.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TemplatedPathList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplatedPathList\"\n        },\n        {\n          \"description\": \"The config's templated path list.\"\n        }\n      ]\n    },\n    \"HistoricalDataPathList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoricalDataPathList\"\n        },\n        {\n          \"description\": \"The config's historical data path list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-auto-detection-s3-source-config-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AutoDetectionS3SourceConfig
---
