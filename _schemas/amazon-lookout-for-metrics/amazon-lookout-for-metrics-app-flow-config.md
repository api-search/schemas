---
description: Details about an Amazon AppFlow flow datasource.
layout: schema
name: AppFlowConfig
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: FlowName
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-app-flow-config-schema.json
slug: amazon-lookout-for-metrics-app-flow-config
source_filename: amazon-lookout-for-metrics-app-flow-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-app-flow-config-schema.json\",\n  \"title\": \"AppFlowConfig\",\n  \"description\": \"Details about an Amazon AppFlow flow datasource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"An IAM role that gives Amazon Lookout for Metrics permission to access the flow.\"\n        }\n      ]\n    },\n    \"FlowName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlowName\"\n        },\n        {\n          \"description\": \" name of the flow.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-app-flow-config-schema.json
tags:
- Anomaly Detection
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: AppFlowConfig
---
