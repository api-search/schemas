---
description: Repository containing the source code for a pipeline.
layout: schema
name: CodeRepository
properties_list:
- description: Authorization info to access the code repository.
  name: authorization
  type: object
- description: Default branch used to configure Continuous Integration (CI) in the pipeline.
  name: defaultBranch
  type: string
- description: Unique immutable identifier of the code repository.
  name: id
  type: string
- description: Repository-specific properties.
  name: properties
  type: object
- description: Type of code repository.
  name: repositoryType
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-code-repository-schema.json
slug: azure-dev-ops-code-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-code-repository-schema.json\",\n  \"title\": \"CodeRepository\",\n  \"description\": \"Repository containing the source code for a pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorization\": {\n      \"$ref\": \"#/definitions/Authorization\",\n      \"description\": \"Authorization info to access the code repository.\"\n    },\n    \"defaultBranch\": {\n      \"description\": \"Default branch used to configure Continuous Integration (CI) in the pipeline.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Unique immutable identifier of the code repository.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Repository-specific properties.\"\
  ,\n      \"type\": \"object\",\n      \"x-ms-client-flatten\": true\n    },\n    \"repositoryType\": {\n      \"description\": \"Type of code repository.\",\n      \"enum\": [\n        \"gitHub\",\n        \"vstsGit\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"CodeRepositoryType\"\n      }\n    }\n  },\n  \"required\": [\n    \"repositoryType\",\n    \"id\",\n    \"defaultBranch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-dev-ops/refs/heads/main/json-schema/azure-dev-ops-code-repository-schema.json
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: CodeRepository
---
