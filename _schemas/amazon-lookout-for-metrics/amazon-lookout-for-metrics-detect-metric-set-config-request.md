---
description: DetectMetricSetConfigRequest schema from Amazon Lookout for Metrics API
layout: schema
name: DetectMetricSetConfigRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: AutoDetectionMetricSource
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-detect-metric-set-config-request-schema.json
slug: amazon-lookout-for-metrics-detect-metric-set-config-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detect-metric-set-config-request-schema.json\",\n  \"title\": \"DetectMetricSetConfigRequest\",\n  \"description\": \"DetectMetricSetConfigRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"An anomaly detector ARN.\"\n        }\n      ]\n    },\n    \"AutoDetectionMetricSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoDetectionMetricSource\"\n        },\n        {\n          \"description\": \"A data source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\",\n    \"AutoDetectionMetricSource\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-detect-metric-set-config-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DetectMetricSetConfigRequest
---
