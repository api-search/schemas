---
description: GetRecommendationSummariesResponse schema
layout: schema
name: GetRecommendationSummariesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: recommendationSummaries
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-recommendation-summaries-response-schema.json
slug: compute-optimizer-get-recommendation-summaries-response
source_filename: compute-optimizer-get-recommendation-summaries-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-summaries-response-schema.json\",\n  \"title\": \"GetRecommendationSummariesResponse\",\n  \"description\": \"GetRecommendationSummariesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"<p>The token to use to advance to the next page of recommendation summaries.</p> <p>This value is null when there are no more pages of recommendation summaries to return.</p>\"\n        }\n      ]\n    },\n    \"recommendationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSummaries\"\n        },\n        {\n          \"description\": \"An array\
  \ of objects that summarize a recommendation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-summaries-response-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetRecommendationSummariesResponse
---
