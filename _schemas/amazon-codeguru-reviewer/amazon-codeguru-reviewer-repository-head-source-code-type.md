---
description: A <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType">SourceCodeType</a> that specifies the tip of a branch in an associated repository.
layout: schema
name: RepositoryHeadSourceCodeType
properties_list:
- description: ''
  name: BranchName
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-repository-head-source-code-type-schema.json
slug: amazon-codeguru-reviewer-repository-head-source-code-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-head-source-code-type-schema.json\",\n  \"title\": \"RepositoryHeadSourceCodeType\",\n  \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies the tip of a branch in an associated repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BranchName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BranchName\"\n        },\n        {\n          \"description\": \"The name of the branch in an associated repository. The <code>RepositoryHeadSourceCodeType</code> specifies the tip of this branch.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BranchName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-repository-head-source-code-type-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RepositoryHeadSourceCodeType
---
