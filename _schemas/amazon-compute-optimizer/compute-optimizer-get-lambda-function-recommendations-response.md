---
description: GetLambdaFunctionRecommendationsResponse schema
layout: schema
name: GetLambdaFunctionRecommendationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: lambdaFunctionRecommendations
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-lambda-function-recommendations-response-schema.json
slug: compute-optimizer-get-lambda-function-recommendations-response
source_filename: compute-optimizer-get-lambda-function-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-lambda-function-recommendations-response-schema.json\",\n  \"title\": \"GetLambdaFunctionRecommendationsResponse\",\n  \"description\": \"GetLambdaFunctionRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of function recommendations.</p> <p>This value is null when there are no more pages of function recommendations to return.</p>\"\n        }\n      ]\n    },\n    \"lambdaFunctionRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecommendations\"\n        },\n        {\n      \
  \    \"description\": \"An array of objects that describe function recommendations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-lambda-function-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetLambdaFunctionRecommendationsResponse
---
