---
description: UpdateAnomalyDetectorResponse schema from Amazon Lookout for Metrics API
layout: schema
name: UpdateAnomalyDetectorResponse
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-update-anomaly-detector-response-schema.json
slug: amazon-lookout-for-metrics-update-anomaly-detector-response
source_filename: amazon-lookout-for-metrics-update-anomaly-detector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-anomaly-detector-response-schema.json\",\n  \"title\": \"UpdateAnomalyDetectorResponse\",\n  \"description\": \"UpdateAnomalyDetectorResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the updated detector.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-anomaly-detector-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: UpdateAnomalyDetectorResponse
---
