---
description: Contains information about a detector's configuration.
layout: schema
name: AnomalyDetectorConfig
properties_list:
- description: ''
  name: AnomalyDetectorFrequency
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-detector-config-schema.json
slug: amazon-lookout-for-metrics-anomaly-detector-config
source_filename: amazon-lookout-for-metrics-anomaly-detector-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-config-schema.json\",\n  \"title\": \"AnomalyDetectorConfig\",\n  \"description\": \"Contains information about a detector's configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"The frequency at which the detector analyzes its source data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-config-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyDetectorConfig
---
