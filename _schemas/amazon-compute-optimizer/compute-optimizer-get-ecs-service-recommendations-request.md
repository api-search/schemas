---
description: GetECSServiceRecommendationsRequest schema
layout: schema
name: GetECSServiceRecommendationsRequest
properties_list:
- description: ''
  name: serviceArns
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: filters
  type: object
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ecs-service-recommendations-request-schema.json
slug: compute-optimizer-get-ecs-service-recommendations-request
source_filename: compute-optimizer-get-ecs-service-recommendations-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendations-request-schema.json\",\n  \"title\": \"GetECSServiceRecommendationsRequest\",\n  \"description\": \"GetECSServiceRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceArns\"\n        },\n        {\n          \"description\": \"<p> The ARN that identifies the Amazon ECS service. </p> <p> The following is the format of the ARN: </p> <p> <code>arn:aws:ecs:region:aws_account_id:service/cluster-name/service-name</code> </p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \" The token\
  \ to advance to the next page of Amazon ECS service recommendations. \"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p> The maximum number of Amazon ECS service recommendations to return with a single request. </p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSServiceRecommendationFilters\"\n        },\n        {\n          \"description\": \" An array of objects to specify a filter that returns a more specific list of Amazon ECS service recommendations. \"\n        }\n      ]\n    },\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p> Return\
  \ the Amazon ECS service recommendations to the specified Amazon Web Services account IDs. </p> <p>If your account is the management account or the delegated administrator of an organization, use this parameter to return the Amazon ECS service recommendations to specific member accounts.</p> <p>You can only specify one account ID per request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ecs-service-recommendations-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetECSServiceRecommendationsRequest
---
