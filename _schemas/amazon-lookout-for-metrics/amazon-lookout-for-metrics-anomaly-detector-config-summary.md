---
description: Contains information about a detector's configuration.
layout: schema
name: AnomalyDetectorConfigSummary
properties_list:
- description: ''
  name: AnomalyDetectorFrequency
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-detector-config-summary-schema.json
slug: amazon-lookout-for-metrics-anomaly-detector-config-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-config-summary-schema.json\",\n  \"title\": \"AnomalyDetectorConfigSummary\",\n  \"description\": \"Contains information about a detector's configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorFrequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Frequency\"\n        },\n        {\n          \"description\": \"The interval at which the detector analyzes its source data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-config-summary-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyDetectorConfigSummary
---
