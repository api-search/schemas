---
description: Describes the recommendation options for an Amazon ECS service.
layout: schema
name: ECSServiceRecommendationOption
properties_list:
- description: ''
  name: memory
  type: object
- description: ''
  name: cpu
  type: object
- description: ''
  name: savingsOpportunity
  type: object
- description: ''
  name: projectedUtilizationMetrics
  type: object
- description: ''
  name: containerRecommendations
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-recommendation-option-schema.json
slug: compute-optimizer-ecs-service-recommendation-option
source_filename: compute-optimizer-ecs-service-recommendation-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-option-schema.json\",\n  \"title\": \"ECSServiceRecommendationOption\",\n  \"description\": \" Describes the recommendation options for an Amazon ECS service. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"memory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableMemory\"\n        },\n        {\n          \"description\": \" The memory size of the Amazon ECS service recommendation option. \"\n        }\n      ]\n    },\n    \"cpu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableCpu\"\n        },\n        {\n          \"description\": \" The CPU size of the Amazon ECS service recommendation option. \"\n        }\n      ]\n    },\n    \"savingsOpportunity\": {\n    \
  \  \"$ref\": \"#/components/schemas/SavingsOpportunity\"\n    },\n    \"projectedUtilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceProjectedUtilizationMetrics\"\n        },\n        {\n          \"description\": \" An array of objects that describe the projected utilization metrics of the Amazon ECS service recommendation option. \"\n        }\n      ]\n    },\n    \"containerRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContainerRecommendations\"\n        },\n        {\n          \"description\": \" The CPU and memory size recommendations for the containers within the task of your Amazon ECS service. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommendation-option-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceRecommendationOption
---
