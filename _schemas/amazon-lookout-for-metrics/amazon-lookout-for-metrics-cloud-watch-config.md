---
description: Details about an Amazon CloudWatch datasource.
layout: schema
name: CloudWatchConfig
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: BackTestConfiguration
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-cloud-watch-config-schema.json
slug: amazon-lookout-for-metrics-cloud-watch-config
source_filename: amazon-lookout-for-metrics-cloud-watch-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-cloud-watch-config-schema.json\",\n  \"title\": \"CloudWatchConfig\",\n  \"description\": \"Details about an Amazon CloudWatch datasource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"An IAM role that gives Amazon Lookout for Metrics permission to access data in Amazon CloudWatch.\"\n        }\n      ]\n    },\n    \"BackTestConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BackTestConfiguration\"\n        },\n        {\n          \"description\": \"Settings for backtest mode.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-cloud-watch-config-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CloudWatchConfig
---
