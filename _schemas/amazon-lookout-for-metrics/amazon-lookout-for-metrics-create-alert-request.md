---
description: CreateAlertRequest schema from Amazon Lookout for Metrics API
layout: schema
name: CreateAlertRequest
properties_list:
- description: ''
  name: AlertName
  type: object
- description: ''
  name: AlertSensitivityThreshold
  type: object
- description: ''
  name: AlertDescription
  type: object
- description: ''
  name: AnomalyDetectorArn
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: AlertFilters
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-create-alert-request-schema.json
slug: amazon-lookout-for-metrics-create-alert-request
source_filename: amazon-lookout-for-metrics-create-alert-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-alert-request-schema.json\",\n  \"title\": \"CreateAlertRequest\",\n  \"description\": \"CreateAlertRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertName\"\n        },\n        {\n          \"description\": \"The name of the alert.\"\n        }\n      ]\n    },\n    \"AlertSensitivityThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityThreshold\"\n        },\n        {\n          \"description\": \"An integer from 0 to 100 specifying the alert sensitivity threshold.\"\n        }\n      ]\n    },\n    \"AlertDescription\": {\n      \"allOf\": [\n        {\n   \
  \       \"$ref\": \"#/components/schemas/AlertDescription\"\n        },\n        {\n          \"description\": \"A description of the alert.\"\n        }\n      ]\n    },\n    \"AnomalyDetectorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the detector to which the alert is attached.\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"Action that will be triggered when there is an alert.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of <a href=\\\"https://docs.aws.amazon.com/lookoutmetrics/latest/dev/detectors-tags.html\\\">tags</a> to apply to the alert.\"\n        }\n      ]\n    },\n    \"AlertFilters\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertFilters\"\n        },\n        {\n          \"description\": \"The configuration of the alert filters, containing MetricList and DimensionFilterList.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AlertName\",\n    \"AnomalyDetectorArn\",\n    \"Action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-create-alert-request-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: CreateAlertRequest
---
