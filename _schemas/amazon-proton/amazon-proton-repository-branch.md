---
description: Detail data for a linked repository branch.
layout: schema
name: RepositoryBranch
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: branch
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: provider
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-repository-branch-schema.json
slug: amazon-proton-repository-branch
source_filename: amazon-proton-repository-branch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-branch-schema.json\",\n  \"title\": \"RepositoryBranch\",\n  \"description\": \"Detail data for a linked repository branch.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the linked repository.\"\n        }\n      ]\n    },\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The repository branch.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\"\
  : \"The repository name.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"arn\",\n    \"branch\",\n    \"name\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-branch-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: RepositoryBranch
---
