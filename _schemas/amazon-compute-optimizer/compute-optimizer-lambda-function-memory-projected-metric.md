---
description: Describes a projected utilization metric of an Lambda function recommendation option.
layout: schema
name: LambdaFunctionMemoryProjectedMetric
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: statistic
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-lambda-function-memory-projected-metric-schema.json
slug: compute-optimizer-lambda-function-memory-projected-metric
source_filename: compute-optimizer-lambda-function-memory-projected-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-memory-projected-metric-schema.json\",\n  \"title\": \"LambdaFunctionMemoryProjectedMetric\",\n  \"description\": \"Describes a projected utilization metric of an Lambda function recommendation option.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionMemoryMetricName\"\n        },\n        {\n          \"description\": \"The name of the projected utilization metric.\"\n        }\n      ]\n    },\n    \"statistic\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionMemoryMetricStatistic\"\n        },\n        {\n          \"description\": \"The statistic of the projected utilization metric.\"\n        }\n      ]\n  \
  \  },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricValue\"\n        },\n        {\n          \"description\": \"The values of the projected utilization metrics.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-memory-projected-metric-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: LambdaFunctionMemoryProjectedMetric
---
