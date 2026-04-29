---
description: Information about an Amazon Web Services CodeCommit repository. The CodeCommit repository must be in the same Amazon Web Services Region and Amazon Web Services account where its CodeGuru Reviewer code reviews are configured.
layout: schema
name: CodeCommitRepository
properties_list:
- description: ''
  name: Name
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-code-commit-repository-schema.json
slug: amazon-codeguru-reviewer-code-commit-repository
source_filename: amazon-codeguru-reviewer-code-commit-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-commit-repository-schema.json\",\n  \"title\": \"CodeCommitRepository\",\n  \"description\": \"Information about an Amazon Web Services CodeCommit repository. The CodeCommit repository must be in the same Amazon Web Services Region and Amazon Web Services account where its CodeGuru Reviewer code reviews are configured.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the Amazon Web Services CodeCommit repository. For more information, see <a href=\\\"https://docs.aws.amazon.com/codecommit/latest/APIReference/API_GetRepository.html#CodeCommit-GetRepository-request-repositoryName\\\">repositoryName</a> in\
  \ the <i>Amazon Web Services CodeCommit API Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-commit-repository-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CodeCommitRepository
---
