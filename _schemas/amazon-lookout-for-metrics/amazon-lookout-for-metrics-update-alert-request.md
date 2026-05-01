---
description: UpdateAlertRequest schema from Amazon Lookout for Metrics API
layout: schema
name: UpdateAlertRequest
properties_list:
- description: ''
  name: AlertArn
  type: object
- description: ''
  name: AlertDescription
  type: object
- description: ''
  name: AlertSensitivityThreshold
  type: object
- description: ''
  name: Action
  type: object
- description: ''
  name: AlertFilters
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-update-alert-request-schema.json
slug: amazon-lookout-for-metrics-update-alert-request
source_filename: amazon-lookout-for-metrics-update-alert-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-alert-request-schema.json\",\n  \"title\": \"UpdateAlertRequest\",\n  \"description\": \"UpdateAlertRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the alert to update.\"\n        }\n      ]\n    },\n    \"AlertDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertDescription\"\n        },\n        {\n          \"description\": \"A description of the alert.\"\n        }\n      ]\n    },\n    \"AlertSensitivityThreshold\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitivityThreshold\"\
  \n        },\n        {\n          \"description\": \"An integer from 0 to 100 specifying the alert sensitivity threshold.\"\n        }\n      ]\n    },\n    \"Action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Action\"\n        },\n        {\n          \"description\": \"Action that will be triggered when there is an alert.\"\n        }\n      ]\n    },\n    \"AlertFilters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertFilters\"\n        },\n        {\n          \"description\": \"The configuration of the alert filters, containing MetricList and DimensionFilterList.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AlertArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-update-alert-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: UpdateAlertRequest
---
