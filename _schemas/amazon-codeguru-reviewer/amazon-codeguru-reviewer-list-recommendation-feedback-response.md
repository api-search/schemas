---
description: ListRecommendationFeedbackResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: ListRecommendationFeedbackResponse
properties_list:
- description: ''
  name: RecommendationFeedbackSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-list-recommendation-feedback-response-schema.json
slug: amazon-codeguru-reviewer-list-recommendation-feedback-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-recommendation-feedback-response-schema.json\",\n  \"title\": \"ListRecommendationFeedbackResponse\",\n  \"description\": \"ListRecommendationFeedbackResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecommendationFeedbackSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationFeedbackSummaries\"\n        },\n        {\n          \"description\": \"Recommendation feedback summaries corresponding to the code review ARN.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If <code>nextToken</code> is returned, there are more results\
  \ available. The value of <code>nextToken</code> is a unique pagination token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-recommendation-feedback-response-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: ListRecommendationFeedbackResponse
---
