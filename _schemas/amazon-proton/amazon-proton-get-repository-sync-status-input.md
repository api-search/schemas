---
description: GetRepositorySyncStatusInput schema from Amazon Proton API
layout: schema
name: GetRepositorySyncStatusInput
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: repositoryName
  type: object
- description: ''
  name: repositoryProvider
  type: object
- description: ''
  name: syncType
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-get-repository-sync-status-input-schema.json
slug: amazon-proton-get-repository-sync-status-input
source_filename: amazon-proton-get-repository-sync-status-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-sync-status-input-schema.json\",\n  \"title\": \"GetRepositorySyncStatusInput\",\n  \"description\": \"GetRepositorySyncStatusInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The repository branch.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The repository name.\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n       \
  \ },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    },\n    \"syncType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncType\"\n        },\n        {\n          \"description\": \"The repository sync type.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"branch\",\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"syncType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-get-repository-sync-status-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: GetRepositorySyncStatusInput
---
