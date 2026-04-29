---
description: GetAnomalyGroupRequest schema from Amazon Lookout for Metrics API
layout: schema
name: GetAnomalyGroupRequest
properties_list:
- description: ''
  name: AnomalyGroupId
  type: object
- description: ''
  name: AnomalyDetectorArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-get-anomaly-group-request-schema.json
slug: amazon-lookout-for-metrics-get-anomaly-group-request
source_filename: amazon-lookout-for-metrics-get-anomaly-group-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-anomaly-group-request-schema.json\",\n  \"title\": \"GetAnomalyGroupRequest\",\n  \"description\": \"GetAnomalyGroupRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"The ID of the anomaly group.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the anomaly detector.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyGroupId\",\n    \"AnomalyDetectorArn\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-get-anomaly-group-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: GetAnomalyGroupRequest
---
