---
description: DescribeAnomalyDetectorResponse schema from Amazon Lookout for Metrics API
layout: schema
name: DescribeAnomalyDetectorResponse
properties_list:
- description: ''
  name: AnomalyDetectorArn
  type: object
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
  name: CreationTime
  type: object
- description: ''
  name: LastModificationTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: FailureReason
  type: object
- description: ''
  name: KmsKeyArn
  type: object
- description: ''
  name: FailureType
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-describe-anomaly-detector-response-schema.json
slug: amazon-lookout-for-metrics-describe-anomaly-detector-response
source_filename: amazon-lookout-for-metrics-describe-anomaly-detector-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-anomaly-detector-response-schema.json\",\n  \"title\": \"DescribeAnomalyDetectorResponse\",\n  \"description\": \"DescribeAnomalyDetectorResponse schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorName\"\n        },\n        {\n          \"description\": \"The name of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorDescription\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/AnomalyDetectorDescription\"\n        },\n        {\n          \"description\": \"A description of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorConfigSummary\"\n        },\n        {\n          \"description\": \"Contains information about the detector's configuration.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the detector was created.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the detector was last modified.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorStatus\"\n        },\n        {\n          \"description\": \"The status of the detector.\"\n        }\n      ]\n    },\n    \"FailureReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorMessage\"\n        },\n        {\n          \"description\": \"The reason that the detector failed.\"\n        }\n      ]\n    },\n    \"KmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyArn\"\n        },\n        {\n          \"description\": \"The ARN of the KMS key to use to encrypt your data.\"\n        }\n      ]\n    },\n    \"FailureType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorFailureType\"\n        },\n        {\n          \"description\": \"The process that caused the detector to fail.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-describe-anomaly-detector-response-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DescribeAnomalyDetectorResponse
---
