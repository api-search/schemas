---
description: Provides a summary of an alert's configuration.
layout: schema
name: AlertSummary
properties_list:
- description: ''
  name: AlertArn
  type: object
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: AlertName
  type: object
- description: ''
  name: AlertSensitivityThreshold
  type: object
- description: ''
  name: AlertType
  type: object
- description: ''
  name: AlertStatus
  type: object
- description: ''
  name: LastModificationTime
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-alert-summary-schema.json
slug: amazon-lookout-for-metrics-alert-summary
source_filename: amazon-lookout-for-metrics-alert-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-summary-schema.json\",\n  \"title\": \"AlertSummary\",\n  \"description\": \"Provides a summary of an alert's configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the alert.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector to which the alert is attached.\"\n        }\n      ]\n    },\n    \"AlertName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertName\"\n        },\n        {\n   \
  \       \"description\": \"The name of the alert.\"\n        }\n      ]\n    },\n    \"AlertSensitivityThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityThreshold\"\n        },\n        {\n          \"description\": \"The minimum severity for an anomaly to trigger the alert.\"\n        }\n      ]\n    },\n    \"AlertType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertType\"\n        },\n        {\n          \"description\": \"The type of the alert.\"\n        }\n      ]\n    },\n    \"AlertStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertStatus\"\n        },\n        {\n          \"description\": \"The status of the alert.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the alert was last\
  \ modified.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the alert was created.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The alert's <a href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-summary-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AlertSummary
---
