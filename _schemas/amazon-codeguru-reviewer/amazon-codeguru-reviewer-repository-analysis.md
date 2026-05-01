---
description: A code review type that analyzes all code under a specified branch in an associated repository. The associated repository is specified using its ARN when you call <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CreateCodeReview">CreateCodeReview</a>.
layout: schema
name: RepositoryAnalysis
properties_list:
- description: ''
  name: RepositoryHead
  type: object
- description: ''
  name: SourceCodeType
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-repository-analysis-schema.json
slug: amazon-codeguru-reviewer-repository-analysis
source_filename: amazon-codeguru-reviewer-repository-analysis-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-analysis-schema.json\",\n  \"title\": \"RepositoryAnalysis\",\n  \"description\": \"A code review type that analyzes all code under a specified branch in an associated repository. The associated repository is specified using its ARN when you call <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CreateCodeReview\\\">CreateCodeReview</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RepositoryHead\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryHeadSourceCodeType\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies the tip of a branch in an associated repository.\"\
  \n        }\n      ]\n    },\n    \"SourceCodeType\": {\n      \"$ref\": \"#/components/schemas/SourceCodeType\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-analysis-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RepositoryAnalysis
---
