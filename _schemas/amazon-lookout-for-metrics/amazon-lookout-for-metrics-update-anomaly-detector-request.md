---
description: UpdateAnomalyDetectorRequest schema from Amazon Lookout for Metrics API
layout: schema
name: UpdateAnomalyDetectorRequest
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: AnomalyDetectorDescription
  type: object
- description: ''
  name: AnomalyDetectorConfig
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-update-anomaly-detector-request-schema.json
slug: amazon-lookout-for-metrics-update-anomaly-detector-request
source_filename: amazon-lookout-for-metrics-update-anomaly-detector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-anomaly-detector-request-schema.json\",\n  \"title\": \"UpdateAnomalyDetectorRequest\",\n  \"description\": \"UpdateAnomalyDetectorRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector to update.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of an AWS KMS encryption key.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorDescription\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorDescription\"\n        },\n        {\n          \"description\": \"The updated detector description.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorConfig\"\n        },\n        {\n          \"description\": \"Contains information about the configuration to which the detector will be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-anomaly-detector-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: UpdateAnomalyDetectorRequest
---
