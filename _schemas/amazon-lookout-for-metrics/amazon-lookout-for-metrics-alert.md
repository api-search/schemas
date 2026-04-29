---
description: A configuration for Amazon SNS-integrated notifications.
layout: schema
name: Alert
properties_list:
- description: ''
  name: Action
  type: object
- description: ''
  name: AlertDescription
  type: object
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
  name: AlertFilters
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-alert-schema.json
slug: amazon-lookout-for-metrics-alert
source_filename: amazon-lookout-for-metrics-alert-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-schema.json\",\n  \"title\": \"Alert\",\n  \"description\": \"A configuration for Amazon SNS-integrated notifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"Action that will be triggered when there is an alert.\"\n        }\n      ]\n    },\n    \"AlertDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertDescription\"\n        },\n        {\n          \"description\": \"A description of the alert.\"\n        }\n      ]\n    },\n    \"AlertArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n\
  \          \"description\": \"The ARN of the alert.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector to which the alert is attached.\"\n        }\n      ]\n    },\n    \"AlertName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertName\"\n        },\n        {\n          \"description\": \"The name of the alert.\"\n        }\n      ]\n    },\n    \"AlertSensitivityThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityThreshold\"\n        },\n        {\n          \"description\": \"The minimum severity for an anomaly to trigger the alert.\"\n        }\n      ]\n    },\n    \"AlertType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertType\"\n        },\n        {\n          \"description\": \"The type of the\
  \ alert.\"\n        }\n      ]\n    },\n    \"AlertStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertStatus\"\n        },\n        {\n          \"description\": \"The status of the alert.\"\n        }\n      ]\n    },\n    \"LastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the alert was last modified.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the alert was created.\"\n        }\n      ]\n    },\n    \"AlertFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertFilters\"\n        },\n        {\n          \"description\": \"The configuration of the alert filters, containing MetricList and DimensionFilter.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-alert-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: Alert
---
