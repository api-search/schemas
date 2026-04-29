---
description: Information about recommendation feedback summaries.
layout: schema
name: RecommendationFeedbackSummary
properties_list:
- description: ''
  name: RecommendationId
  type: object
- description: ''
  name: Reactions
  type: object
- description: ''
  name: UserId
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-recommendation-feedback-summary-schema.json
slug: amazon-codeguru-reviewer-recommendation-feedback-summary
source_filename: amazon-codeguru-reviewer-recommendation-feedback-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-recommendation-feedback-summary-schema.json\",\n  \"title\": \"RecommendationFeedbackSummary\",\n  \"description\": \"Information about recommendation feedback summaries.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RecommendationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationId\"\n        },\n        {\n          \"description\": \"The recommendation ID that can be used to track the provided recommendations. Later on it can be used to collect the feedback.\"\n        }\n      ]\n    },\n    \"Reactions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Reactions\"\n        },\n        {\n          \"description\": \"List for storing reactions. Reactions are utf-8 text code for emojis.\"\
  \n        }\n      ]\n    },\n    \"UserId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserId\"\n        },\n        {\n          \"description\": \"<p>The ID of the user that gave the feedback.</p> <p> The <code>UserId</code> is an IAM principal that can be specified as an Amazon Web Services account ID or an Amazon Resource Name (ARN). For more information, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_elements_principal.html#Principal_specifying\\\"> Specifying a Principal</a> in the <i>Amazon Web Services Identity and Access Management User Guide</i>.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-recommendation-feedback-summary-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RecommendationFeedbackSummary
---
