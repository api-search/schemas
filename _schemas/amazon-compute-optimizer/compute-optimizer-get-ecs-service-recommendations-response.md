---
description: GetECSServiceRecommendationsResponse schema
layout: schema
name: GetECSServiceRecommendationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: ecsServiceRecommendations
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ecs-service-recommendations-response-schema.json
slug: compute-optimizer-get-ecs-service-recommendations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendations-response-schema.json\",\n  \"title\": \"GetECSServiceRecommendationsResponse\",\n  \"description\": \"GetECSServiceRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" The token to advance to the next page of Amazon ECS service recommendations. \"\n        }\n      ]\n    },\n    \"ecsServiceRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendations\"\n        },\n        {\n          \"description\": \" An array of objects that describe the Amazon ECS service recommendations. \"\n        }\n   \
  \   ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRecommendationErrors\"\n        },\n        {\n          \"description\": \" An array of objects that describe errors of the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetECSServiceRecommendationsResponse
---
