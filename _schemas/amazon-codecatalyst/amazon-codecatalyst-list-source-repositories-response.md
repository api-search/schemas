---
description: ListSourceRepositoriesResponse schema from Amazon CodeCatalyst
layout: schema
name: ListSourceRepositoriesResponse
properties_list:
- description: ''
  name: items
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-source-repositories-response-schema.json
slug: amazon-codecatalyst-list-source-repositories-response
source_filename: amazon-codecatalyst-list-source-repositories-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-response-schema.json\",\n  \"title\": \"ListSourceRepositoriesResponse\",\n  \"description\": \"ListSourceRepositoriesResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListSourceRepositoriesItems\"\n        },\n        {\n          \"description\": \"Information about the source repositories.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-source-repositories-response-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListSourceRepositoriesResponse
---
