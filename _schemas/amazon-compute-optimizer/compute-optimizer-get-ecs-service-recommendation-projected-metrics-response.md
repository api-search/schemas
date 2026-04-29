---
description: GetECSServiceRecommendationProjectedMetricsResponse schema
layout: schema
name: GetECSServiceRecommendationProjectedMetricsResponse
properties_list:
- description: ''
  name: recommendedOptionProjectedMetrics
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-response-schema.json
slug: compute-optimizer-get-ecs-service-recommendation-projected-metrics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-response-schema.json\",\n  \"title\": \"GetECSServiceRecommendationProjectedMetricsResponse\",\n  \"description\": \"GetECSServiceRecommendationProjectedMetricsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendedOptionProjectedMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendedOptionProjectedMetrics\"\n        },\n        {\n          \"description\": \" An array of objects that describes the projected metrics. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendation-projected-metrics-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetECSServiceRecommendationProjectedMetricsResponse
---
