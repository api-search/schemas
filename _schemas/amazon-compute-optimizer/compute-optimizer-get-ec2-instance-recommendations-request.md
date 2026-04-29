---
description: GetEC2InstanceRecommendationsRequest schema
layout: schema
name: GetEC2InstanceRecommendationsRequest
properties_list:
- description: ''
  name: instanceArns
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
- description: ''
  name: recommendationPreferences
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ec2-instance-recommendations-request-schema.json
slug: compute-optimizer-get-ec2-instance-recommendations-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-instance-recommendations-request-schema.json\",\n  \"title\": \"GetEC2InstanceRecommendationsRequest\",\n  \"description\": \"GetEC2InstanceRecommendationsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArns\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the instances for which to return recommendations.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of instance recommendations.\"\n        }\n      ]\n    },\n    \"maxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of instance recommendations to return with a single request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"An array of objects to specify a filter that returns a more specific list of instance recommendations.\"\n        }\n      ]\n    },\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p>The ID of the Amazon Web Services account for which to return instance recommendations.</p> <p>If your account is the management account of an organization, use this parameter\
  \ to specify the member account for which you want to return instance recommendations.</p> <p>Only one account ID can be specified per request.</p>\"\n        }\n      ]\n    },\n    \"recommendationPreferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationPreferences\"\n        },\n        {\n          \"description\": \"An object to specify the preferences for the Amazon EC2 instance recommendations to return in the response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-instance-recommendations-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEC2InstanceRecommendationsRequest
---
