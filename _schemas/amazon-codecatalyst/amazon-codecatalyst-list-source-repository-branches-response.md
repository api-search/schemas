---
description: ListSourceRepositoryBranchesResponse schema from Amazon CodeCatalyst
layout: schema
name: ListSourceRepositoryBranchesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: items
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-source-repository-branches-response-schema.json
slug: amazon-codecatalyst-list-source-repository-branches-response
source_filename: amazon-codecatalyst-list-source-repository-branches-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repository-branches-response-schema.json\",\n  \"title\": \"ListSourceRepositoryBranchesResponse\",\n  \"description\": \"ListSourceRepositoryBranchesResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n        }\n      ]\n    },\n    \"items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListSourceRepositoryBranchesItems\"\n        },\n        {\n          \"description\": \"Information about the source branches.\"\n        }\n      ]\n    }\n\
  \  },\n  \"required\": [\n    \"items\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repository-branches-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSourceRepositoryBranchesResponse
---
