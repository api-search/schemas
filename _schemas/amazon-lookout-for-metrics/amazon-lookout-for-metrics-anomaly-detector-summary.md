---
description: Contains information about an an anomaly detector.
layout: schema
name: AnomalyDetectorSummary
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
  name: CreationTime
  type: object
- description: ''
  name: LastModificationTime
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-anomaly-detector-summary-schema.json
slug: amazon-lookout-for-metrics-anomaly-detector-summary
source_filename: amazon-lookout-for-metrics-anomaly-detector-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-summary-schema.json\",\n  \"title\": \"AnomalyDetectorSummary\",\n  \"description\": \"Contains information about an an anomaly detector.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorName\"\n        },\n        {\n          \"description\": \"The name of the detector.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorDescription\"\
  \n        },\n        {\n          \"description\": \"A description of the detector.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the detector was created.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the detector was last modified.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnomalyDetectorStatus\"\n        },\n        {\n          \"description\": \"The status of detector.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The detector's\
  \ <a href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-anomaly-detector-summary-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AnomalyDetectorSummary
---
