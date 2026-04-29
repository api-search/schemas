---
description: Describes Compute Optimizer's integration status with your chosen external metric provider. For example, Datadog.
layout: schema
name: ExternalMetricStatus
properties_list:
- description: ''
  name: statusCode
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-external-metric-status-schema.json
slug: compute-optimizer-external-metric-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metric-status-schema.json\",\n  \"title\": \"ExternalMetricStatus\",\n  \"description\": \" Describes Compute Optimizer's integration status with your chosen external metric provider. For example, Datadog. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricStatusCode\"\n        },\n        {\n          \"description\": \" The status code for Compute Optimizer's integration with an external metrics provider. \"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricStatusReason\"\n        },\n        {\n          \"description\": \" The reason for Compute Optimizer's integration\
  \ status with your external metric provider. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-external-metric-status-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ExternalMetricStatus
---
