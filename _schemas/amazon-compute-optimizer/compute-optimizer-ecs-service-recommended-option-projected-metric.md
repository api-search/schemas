---
description: <p> Describes the projected metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the metric data of your service against its projected metric data.</p>
layout: schema
name: ECSServiceRecommendedOptionProjectedMetric
properties_list:
- description: ''
  name: recommendedCpuUnits
  type: object
- description: ''
  name: recommendedMemorySize
  type: object
- description: ''
  name: projectedMetrics
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-ecs-service-recommended-option-projected-metric-schema.json
slug: compute-optimizer-ecs-service-recommended-option-projected-metric
source_filename: compute-optimizer-ecs-service-recommended-option-projected-metric-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommended-option-projected-metric-schema.json\",\n  \"title\": \"ECSServiceRecommendedOptionProjectedMetric\",\n  \"description\": \"<p> Describes the projected metrics of an Amazon ECS service recommendation option. </p> <p>To determine the performance difference between your current Amazon ECS service and the recommended option, compare the metric data of your service against its projected metric data.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendedCpuUnits\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CpuSize\"\n        },\n        {\n          \"description\": \" The recommended CPU size for the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"recommendedMemorySize\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/MemorySize\"\n        },\n        {\n          \"description\": \" The recommended memory size for the Amazon ECS service. \"\n        }\n      ]\n    },\n    \"projectedMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceProjectedMetrics\"\n        },\n        {\n          \"description\": \" An array of objects that describe the projected metric. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-ecs-service-recommended-option-projected-metric-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: ECSServiceRecommendedOptionProjectedMetric
---
