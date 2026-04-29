---
description: ListRecommendationsResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: ListRecommendationsResponse
properties_list:
- description: ''
  name: RecommendationSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-list-recommendations-response-schema.json
slug: amazon-codeguru-reviewer-list-recommendations-response
source_filename: amazon-codeguru-reviewer-list-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-recommendations-response-schema.json\",\n  \"title\": \"ListRecommendationsResponse\",\n  \"description\": \"ListRecommendationsResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecommendationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSummaries\"\n        },\n        {\n          \"description\": \"List of recommendations for the requested code review.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-recommendations-response-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: ListRecommendationsResponse
---
