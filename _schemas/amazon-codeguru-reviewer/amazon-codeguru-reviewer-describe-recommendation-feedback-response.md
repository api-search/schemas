---
description: DescribeRecommendationFeedbackResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: DescribeRecommendationFeedbackResponse
properties_list:
- description: ''
  name: RecommendationFeedback
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-describe-recommendation-feedback-response-schema.json
slug: amazon-codeguru-reviewer-describe-recommendation-feedback-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-describe-recommendation-feedback-response-schema.json\",\n  \"title\": \"DescribeRecommendationFeedbackResponse\",\n  \"description\": \"DescribeRecommendationFeedbackResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecommendationFeedback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationFeedback\"\n        },\n        {\n          \"description\": \"The recommendation feedback given by the user.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-describe-recommendation-feedback-response-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: DescribeRecommendationFeedbackResponse
---
