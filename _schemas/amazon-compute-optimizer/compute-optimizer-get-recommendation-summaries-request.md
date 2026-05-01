---
description: GetRecommendationSummariesRequest schema
layout: schema
name: GetRecommendationSummariesRequest
properties_list:
- description: ''
  name: accountIds
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-get-recommendation-summaries-request-schema.json
slug: compute-optimizer-get-recommendation-summaries-request
source_filename: compute-optimizer-get-recommendation-summaries-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-summaries-request-schema.json\",\n  \"title\": \"GetRecommendationSummariesRequest\",\n  \"description\": \"GetRecommendationSummariesRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIds\"\n        },\n        {\n          \"description\": \"<p>The ID of the Amazon Web Services account for which to return recommendation summaries.</p> <p>If your account is the management account of an organization, use this parameter to specify the member account for which you want to return recommendation summaries.</p> <p>Only one account ID can be specified per request.</p>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n      \
  \  {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The token to advance to the next page of recommendation summaries.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"<p>The maximum number of recommendation summaries to return with a single request.</p> <p>To retrieve the remaining results, make another request with the returned <code>nextToken</code> value.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-get-recommendation-summaries-request-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: GetRecommendationSummariesRequest
---
