---
description: The repository to be created in AWS CodeStar. Valid values are AWS CodeCommit or GitHub. After AWS CodeStar provisions the new repository, the source code files provided with the project request are placed in the repository.
layout: schema
name: CodeDestination
properties_list:
- description: ''
  name: codeCommit
  type: object
- description: ''
  name: gitHub
  type: object
provider_name: Amazon CodeStar
provider_slug: amazon-codestar
schema_file: json-schema/codestar-code-destination-schema.json
slug: codestar-code-destination
source_filename: codestar-code-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-destination-schema.json\",\n  \"title\": \"CodeDestination\",\n  \"description\": \"The repository to be created in AWS CodeStar. Valid values are AWS CodeCommit or GitHub. After AWS CodeStar provisions the new repository, the source code files provided with the project request are placed in the repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"codeCommit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeCommitCodeDestination\"\n        },\n        {\n          \"description\": \"Information about the AWS CodeCommit repository to be created in AWS CodeStar. This is where the source code files provided with the project request will be uploaded after project creation.\"\n        }\n      ]\n    },\n    \"gitHub\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/GitHubCodeDestination\"\n        },\n        {\n          \"description\": \"Information about the GitHub repository to be created in AWS CodeStar. This is where the source code files provided with the project request will be uploaded after project creation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codestar/refs/heads/main/json-schema/codestar-code-destination-schema.json
tags:
- Developer Tools
- DevOps
- Project Management
- Team Collaboration
title: CodeDestination
---
