---
description: CreateAnomalyDetectorRequest schema from Amazon Lookout for Metrics API
layout: schema
name: CreateAnomalyDetectorRequest
properties_list:
- description: ''
  name: AnomalyDetectorName
  type: object
- description: ''
  name: AnomalyDetectorDescription
  type: object
- description: ''
  name: AnomalyDetectorConfig
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-create-anomaly-detector-request-schema.json
slug: amazon-lookout-for-metrics-create-anomaly-detector-request
source_filename: amazon-lookout-for-metrics-create-anomaly-detector-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-anomaly-detector-request-schema.json\",\n  \"title\": \"CreateAnomalyDetectorRequest\",\n  \"description\": \"CreateAnomalyDetectorRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorName\"\n        },\n        {\n          \"description\": \"The name of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorDescription\"\n        },\n        {\n          \"description\": \"A description of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorConfig\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorConfig\"\n        },\n        {\n          \"description\": \"Contains information about the configuration of the anomaly detector.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The ARN of the KMS key to use to encrypt your data.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of <a href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a> to apply to the anomaly detector.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AnomalyDetectorName\",\n    \"AnomalyDetectorConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-anomaly-detector-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CreateAnomalyDetectorRequest
---
