---
description: PutRecommendationFeedbackRequest schema from Amazon CodeGuru Reviewer
layout: schema
name: PutRecommendationFeedbackRequest
properties_list:
- description: ''
  name: CodeReviewArn
  type: object
- description: ''
  name: RecommendationId
  type: object
- description: ''
  name: Reactions
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-put-recommendation-feedback-request-schema.json
slug: amazon-codeguru-reviewer-put-recommendation-feedback-request
source_filename: amazon-codeguru-reviewer-put-recommendation-feedback-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-put-recommendation-feedback-request-schema.json\",\n  \"title\": \"PutRecommendationFeedbackRequest\",\n  \"description\": \"PutRecommendationFeedbackRequest schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeReviewArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReview.html\\\">CodeReview</a> object. \"\n        }\n      ]\n    },\n    \"RecommendationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationId\"\n        },\n        {\n          \"description\": \"The recommendation\
  \ ID that can be used to track the provided recommendations and then to collect the feedback.\"\n        }\n      ]\n    },\n    \"Reactions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reactions\"\n        },\n        {\n          \"description\": \"List for storing reactions. Reactions are utf-8 text code for emojis. If you send an empty list it clears all your feedback.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"CodeReviewArn\",\n    \"RecommendationId\",\n    \"Reactions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-put-recommendation-feedback-request-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: PutRecommendationFeedbackRequest
---
