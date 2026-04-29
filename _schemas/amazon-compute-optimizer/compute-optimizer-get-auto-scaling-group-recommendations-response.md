---
description: GetAutoScalingGroupRecommendationsResponse schema
layout: schema
name: GetAutoScalingGroupRecommendationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: autoScalingGroupRecommendations
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-auto-scaling-group-recommendations-response-schema.json
slug: compute-optimizer-get-auto-scaling-group-recommendations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-auto-scaling-group-recommendations-response-schema.json\",\n  \"title\": \"GetAutoScalingGroupRecommendationsResponse\",\n  \"description\": \"GetAutoScalingGroupRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of Auto Scaling group recommendations.</p> <p>This value is null when there are no more pages of Auto Scaling group recommendations to return.</p>\"\n        }\n      ]\n    },\n    \"autoScalingGroupRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoScalingGroupRecommendations\"\n\
  \        },\n        {\n          \"description\": \"An array of objects that describe Auto Scaling group recommendations.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRecommendationErrors\"\n        },\n        {\n          \"description\": \"<p>An array of objects that describe errors of the request.</p> <p>For example, an error is returned if you request recommendations for an unsupported Auto Scaling group.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-auto-scaling-group-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetAutoScalingGroupRecommendationsResponse
---
