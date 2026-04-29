---
description: Describes the source of a recommendation, such as an Amazon EC2 instance or Auto Scaling group.
layout: schema
name: RecommendationSource
properties_list:
- description: ''
  name: recommendationSourceArn
  type: object
- description: ''
  name: recommendationSourceType
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-recommendation-source-schema.json
slug: compute-optimizer-recommendation-source
source_filename: compute-optimizer-recommendation-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-source-schema.json\",\n  \"title\": \"RecommendationSource\",\n  \"description\": \"Describes the source of a recommendation, such as an Amazon EC2 instance or Auto Scaling group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recommendationSourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the recommendation source.\"\n        }\n      ]\n    },\n    \"recommendationSourceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSourceType\"\n        },\n        {\n          \"description\": \"The resource type of the recommendation source.\"\n        }\n      ]\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-recommendation-source-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: RecommendationSource
---
