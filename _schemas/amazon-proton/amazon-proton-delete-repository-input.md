---
description: DeleteRepositoryInput schema from Amazon Proton API
layout: schema
name: DeleteRepositoryInput
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: provider
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-delete-repository-input-schema.json
slug: amazon-proton-delete-repository-input
source_filename: amazon-proton-delete-repository-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-repository-input-schema.json\",\n  \"title\": \"DeleteRepositoryInput\",\n  \"description\": \"DeleteRepositoryInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"The repository name.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"provider\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-delete-repository-input-schema.json
tags:
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: DeleteRepositoryInput
---
