---
description: ListRepositorySyncDefinitionsInput schema from Amazon Proton API
layout: schema
name: ListRepositorySyncDefinitionsInput
properties_list:
- description: ''
  name: nextToken
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
schema_file: json-schema/amazon-proton-list-repository-sync-definitions-input-schema.json
slug: amazon-proton-list-repository-sync-definitions-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repository-sync-definitions-input-schema.json\",\n  \"title\": \"ListRepositorySyncDefinitionsInput\",\n  \"description\": \"ListRepositorySyncDefinitionsInput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next repository sync definition in the array of repository sync definitions, after the list of repository sync definitions previously requested.\"\n        }\n      ]\n    },\n    \"repositoryName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryName\"\n        },\n        {\n          \"description\": \"\
  The repository name.\"\n        }\n      ]\n    },\n    \"repositoryProvider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryProvider\"\n        },\n        {\n          \"description\": \"The repository provider.\"\n        }\n      ]\n    },\n    \"syncType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SyncType\"\n        },\n        {\n          \"description\": \"The sync type. The only supported value is <code>TEMPLATE_SYNC</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"repositoryName\",\n    \"repositoryProvider\",\n    \"syncType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repository-sync-definitions-input-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListRepositorySyncDefinitionsInput
---
