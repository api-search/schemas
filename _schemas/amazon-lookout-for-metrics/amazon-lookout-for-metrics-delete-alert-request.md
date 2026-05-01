---
description: DeleteAlertRequest schema from Amazon Lookout for Metrics API
layout: schema
name: DeleteAlertRequest
properties_list:
- description: ''
  name: AlertArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-delete-alert-request-schema.json
slug: amazon-lookout-for-metrics-delete-alert-request
source_filename: amazon-lookout-for-metrics-delete-alert-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-delete-alert-request-schema.json\",\n  \"title\": \"DeleteAlertRequest\",\n  \"description\": \"DeleteAlertRequest schema from Amazon Lookout for Metrics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AlertArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the alert to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AlertArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-delete-alert-request-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: DeleteAlertRequest
---
