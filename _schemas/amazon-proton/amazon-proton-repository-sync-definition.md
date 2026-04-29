---
description: A repository sync definition.
layout: schema
name: RepositorySyncDefinition
properties_list:
- description: ''
  name: branch
  type: object
- description: ''
  name: directory
  type: object
- description: ''
  name: parent
  type: object
- description: ''
  name: target
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-repository-sync-definition-schema.json
slug: amazon-proton-repository-sync-definition
source_filename: amazon-proton-repository-sync-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-definition-schema.json\",\n  \"title\": \"RepositorySyncDefinition\",\n  \"description\": \"A repository sync definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"branch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GitBranchName\"\n        },\n        {\n          \"description\": \"The repository branch.\"\n        }\n      ]\n    },\n    \"directory\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The directory in the repository.\"\n        }\n      ]\n    },\n    \"parent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The resource that is\
  \ synced from.\"\n        }\n      ]\n    },\n    \"target\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The resource that is synced to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"branch\",\n    \"directory\",\n    \"parent\",\n    \"target\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-repository-sync-definition-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: RepositorySyncDefinition
---
