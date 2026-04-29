---
description: GetEffectiveRecommendationPreferencesRequest schema
layout: schema
name: GetEffectiveRecommendationPreferencesRequest
properties_list:
- description: ''
  name: resourceArn
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-effective-recommendation-preferences-request-schema.json
slug: compute-optimizer-get-effective-recommendation-preferences-request
source_filename: compute-optimizer-get-effective-recommendation-preferences-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-effective-recommendation-preferences-request-schema.json\",\n  \"title\": \"GetEffectiveRecommendationPreferencesRequest\",\n  \"description\": \"GetEffectiveRecommendationPreferencesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource for which to confirm effective recommendation preferences. Only EC2 instance and Auto Scaling group ARNs are currently supported.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-effective-recommendation-preferences-request-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetEffectiveRecommendationPreferencesRequest
---
