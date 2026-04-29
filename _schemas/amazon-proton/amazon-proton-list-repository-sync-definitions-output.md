---
description: ListRepositorySyncDefinitionsOutput schema from Amazon Proton API
layout: schema
name: ListRepositorySyncDefinitionsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: syncDefinitions
  type: object
provider_name: Amazon Proton
provider_slug: amazon-proton
schema_file: json-schema/amazon-proton-list-repository-sync-definitions-output-schema.json
slug: amazon-proton-list-repository-sync-definitions-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repository-sync-definitions-output-schema.json\",\n  \"title\": \"ListRepositorySyncDefinitionsOutput\",\n  \"description\": \"ListRepositorySyncDefinitionsOutput schema from Amazon Proton API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EmptyNextToken\"\n        },\n        {\n          \"description\": \"A token that indicates the location of the next repository sync definition in the array of repository sync definitions, after the current requested list of repository sync definitions.\"\n        }\n      ]\n    },\n    \"syncDefinitions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySyncDefinitionList\"\n        },\n        {\n          \"description\"\
  : \"An array of repository sync definitions.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"syncDefinitions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-proton/refs/heads/main/json-schema/amazon-proton-list-repository-sync-definitions-output-schema.json
tags:
- AWS
- DevOps
- Infrastructure as Code
- Platform Engineering
- Serverless
- Templates
- Self-Service
- CI/CD
title: ListRepositorySyncDefinitionsOutput
---
