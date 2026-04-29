---
description: GetEC2InstanceRecommendationsResponse schema
layout: schema
name: GetEC2InstanceRecommendationsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: instanceRecommendations
  type: object
- description: ''
  name: errors
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-ec2-instance-recommendations-response-schema.json
slug: compute-optimizer-get-ec2-instance-recommendations-response
source_filename: compute-optimizer-get-ec2-instance-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-instance-recommendations-response-schema.json\",\n  \"title\": \"GetEC2InstanceRecommendationsResponse\",\n  \"description\": \"GetEC2InstanceRecommendationsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of instance recommendations.</p> <p>This value is null when there are no more pages of instance recommendations to return.</p>\"\n        }\n      ]\n    },\n    \"instanceRecommendations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRecommendations\"\n        },\n        {\n          \"description\": \"\
  An array of objects that describe instance recommendations.\"\n        }\n      ]\n    },\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRecommendationErrors\"\n        },\n        {\n          \"description\": \"<p>An array of objects that describe errors of the request.</p> <p>For example, an error is returned if you request recommendations for an instance of an unsupported instance family.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-ec2-instance-recommendations-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEC2InstanceRecommendationsResponse
---
