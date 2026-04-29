---
description: DescribeCodeReviewResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: DescribeCodeReviewResponse
properties_list:
- description: ''
  name: CodeReview
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-describe-code-review-response-schema.json
slug: amazon-codeguru-reviewer-describe-code-review-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-describe-code-review-response-schema.json\",\n  \"title\": \"DescribeCodeReviewResponse\",\n  \"description\": \"DescribeCodeReviewResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeReview\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeReview\"\n        },\n        {\n          \"description\": \"Information about the code review.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-describe-code-review-response-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: DescribeCodeReviewResponse
---
