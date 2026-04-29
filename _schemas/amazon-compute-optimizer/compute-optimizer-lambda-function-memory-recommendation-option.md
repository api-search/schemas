---
description: Describes a recommendation option for an Lambda function.
layout: schema
name: LambdaFunctionMemoryRecommendationOption
properties_list:
- description: ''
  name: rank
  type: object
- description: ''
  name: memorySize
  type: object
- description: ''
  name: projectedUtilizationMetrics
  type: object
- description: ''
  name: savingsOpportunity
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-lambda-function-memory-recommendation-option-schema.json
slug: compute-optimizer-lambda-function-memory-recommendation-option
source_filename: compute-optimizer-lambda-function-memory-recommendation-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-memory-recommendation-option-schema.json\",\n  \"title\": \"LambdaFunctionMemoryRecommendationOption\",\n  \"description\": \"Describes a recommendation option for an Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rank\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Rank\"\n        },\n        {\n          \"description\": \"<p>The rank of the function recommendation option.</p> <p>The top recommendation option is ranked as <code>1</code>.</p>\"\n        }\n      ]\n    },\n    \"memorySize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemorySize\"\n        },\n        {\n          \"description\": \"The memory size, in MB, of the function recommendation option.\"\n   \
  \     }\n      ]\n    },\n    \"projectedUtilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionMemoryProjectedMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe the projected utilization metrics of the function recommendation option.\"\n        }\n      ]\n    },\n    \"savingsOpportunity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SavingsOpportunity\"\n        },\n        {\n          \"description\": \"An object that describes the savings opportunity for the Lambda function recommendation option. Savings opportunity includes the estimated monthly savings amount and percentage.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-lambda-function-memory-recommendation-option-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: LambdaFunctionMemoryRecommendationOption
---
