---
description: Contains information about a Lambda configuration.
layout: schema
name: LambdaConfiguration
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: LambdaArn
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-lambda-configuration-schema.json
slug: amazon-lookout-for-metrics-lambda-configuration
source_filename: amazon-lookout-for-metrics-lambda-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-lambda-configuration-schema.json\",\n  \"title\": \"LambdaConfiguration\",\n  \"description\": \"Contains information about a Lambda configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of an IAM role that has permission to invoke the Lambda function.\"\n        }\n      ]\n    },\n    \"LambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the Lambda function.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\",\n    \"LambdaArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-lambda-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: LambdaConfiguration
---
