---
description: Information about the recommendation feedback.
layout: schema
name: RecommendationFeedback
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
- description: ''
  name: UserId
  type: object
- description: ''
  name: CreatedTimeStamp
  type: object
- description: ''
  name: LastUpdatedTimeStamp
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-recommendation-feedback-schema.json
slug: amazon-codeguru-reviewer-recommendation-feedback
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-recommendation-feedback-schema.json\",\n  \"title\": \"RecommendationFeedback\",\n  \"description\": \"Information about the recommendation feedback.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeReviewArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReview.html\\\">CodeReview</a> object. \"\n        }\n      ]\n    },\n    \"RecommendationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationId\"\n        },\n        {\n          \"description\": \"The recommendation ID that can be used to track the provided\
  \ recommendations. Later on it can be used to collect the feedback.\"\n        }\n      ]\n    },\n    \"Reactions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reactions\"\n        },\n        {\n          \"description\": \"List for storing reactions. Reactions are utf-8 text code for emojis. You can send an empty list to clear off all your feedback.\"\n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserId\"\n        },\n        {\n          \"description\": \"<p>The ID of the user that made the API call.</p> <p> The <code>UserId</code> is an IAM principal that can be specified as an Amazon Web Services account ID or an Amazon Resource Name (ARN). For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements_principal.html#Principal_specifying\\\"> Specifying a Principal</a> in the <i>Amazon Web Services Identity and Access Management\
  \ User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"CreatedTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The time at which the feedback was created.\"\n        }\n      ]\n    },\n    \"LastUpdatedTimeStamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"The time at which the feedback was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-recommendation-feedback-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RecommendationFeedback
---
