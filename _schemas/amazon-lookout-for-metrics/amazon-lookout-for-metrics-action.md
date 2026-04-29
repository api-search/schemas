---
description: A configuration that specifies the action to perform when anomalies are detected.
layout: schema
name: Action
properties_list:
- description: ''
  name: SNSConfiguration
  type: object
- description: ''
  name: LambdaConfiguration
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-action-schema.json
slug: amazon-lookout-for-metrics-action
source_filename: amazon-lookout-for-metrics-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"A configuration that specifies the action to perform when anomalies are detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SNSConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SNSConfiguration\"\n        },\n        {\n          \"description\": \"A configuration for an Amazon SNS channel.\"\n        }\n      ]\n    },\n    \"LambdaConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaConfiguration\"\n        },\n        {\n          \"description\": \"A configuration for an AWS Lambda channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-action-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: Action
---
