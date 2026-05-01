---
description: ListCodeReviewsResponse schema from Amazon CodeGuru Reviewer
layout: schema
name: ListCodeReviewsResponse
properties_list:
- description: ''
  name: CodeReviewSummaries
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-list-code-reviews-response-schema.json
slug: amazon-codeguru-reviewer-list-code-reviews-response
source_filename: amazon-codeguru-reviewer-list-code-reviews-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-code-reviews-response-schema.json\",\n  \"title\": \"ListCodeReviewsResponse\",\n  \"description\": \"ListCodeReviewsResponse schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeReviewSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeReviewSummaries\"\n        },\n        {\n          \"description\": \"A list of code reviews that meet the criteria of the request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Pagination token.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-list-code-reviews-response-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: ListCodeReviewsResponse
---
