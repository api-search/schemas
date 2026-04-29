---
description: A type of <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType">SourceCodeType</a> that specifies the commit diff for a pull request on an associated repository. The <code>SourceCommit</code> and <code>DestinationCommit</code> fields are required to do a pull request code review.
layout: schema
name: CommitDiffSourceCodeType
properties_list:
- description: ''
  name: SourceCommit
  type: object
- description: ''
  name: DestinationCommit
  type: object
- description: ''
  name: MergeBaseCommit
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-commit-diff-source-code-type-schema.json
slug: amazon-codeguru-reviewer-commit-diff-source-code-type
source_filename: amazon-codeguru-reviewer-commit-diff-source-code-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-commit-diff-source-code-type-schema.json\",\n  \"title\": \"CommitDiffSourceCodeType\",\n  \"description\": \"A type of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies the commit diff for a pull request on an associated repository. The <code>SourceCommit</code> and <code>DestinationCommit</code> fields are required to do a pull request code review.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceCommit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitId\"\n        },\n        {\n          \"description\": \"The SHA of the source commit used to generate a commit diff. This field is required for a pull request code review.\"\n        }\n      ]\n\
  \    },\n    \"DestinationCommit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitId\"\n        },\n        {\n          \"description\": \"The SHA of the destination commit used to generate a commit diff. This field is required for a pull request code review.\"\n        }\n      ]\n    },\n    \"MergeBaseCommit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitId\"\n        },\n        {\n          \"description\": \"The SHA of the merge base of a commit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-commit-diff-source-code-type-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CommitDiffSourceCodeType
---
