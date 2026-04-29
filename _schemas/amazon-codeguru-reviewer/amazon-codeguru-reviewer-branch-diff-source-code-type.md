---
description: A type of <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType">SourceCodeType</a> that specifies a code diff between a source and destination branch in an associated repository.
layout: schema
name: BranchDiffSourceCodeType
properties_list:
- description: ''
  name: SourceBranchName
  type: object
- description: ''
  name: DestinationBranchName
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-branch-diff-source-code-type-schema.json
slug: amazon-codeguru-reviewer-branch-diff-source-code-type
source_filename: amazon-codeguru-reviewer-branch-diff-source-code-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-branch-diff-source-code-type-schema.json\",\n  \"title\": \"BranchDiffSourceCodeType\",\n  \"description\": \"A type of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies a code diff between a source and destination branch in an associated repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceBranchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BranchName\"\n        },\n        {\n          \"description\": \"The source branch for a diff in an associated repository.\"\n        }\n      ]\n    },\n    \"DestinationBranchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BranchName\"\n        },\n        {\n\
  \          \"description\": \"The destination branch for a diff in an associated repository.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SourceBranchName\",\n    \"DestinationBranchName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-branch-diff-source-code-type-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: BranchDiffSourceCodeType
---
