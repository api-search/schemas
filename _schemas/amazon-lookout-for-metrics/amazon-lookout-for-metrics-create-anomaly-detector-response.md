---
description: CreateAnomalyDetectorResponse schema from Amazon Lookout for Metrics API
layout: schema
name: CreateAnomalyDetectorResponse
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-create-anomaly-detector-response-schema.json
slug: amazon-lookout-for-metrics-create-anomaly-detector-response
source_filename: amazon-lookout-for-metrics-create-anomaly-detector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-anomaly-detector-response-schema.json\",\n  \"title\": \"CreateAnomalyDetectorResponse\",\n  \"description\": \"CreateAnomalyDetectorResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-anomaly-detector-response-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CreateAnomalyDetectorResponse
---
