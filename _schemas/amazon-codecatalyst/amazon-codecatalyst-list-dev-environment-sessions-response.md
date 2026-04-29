---
description: ListDevEnvironmentSessionsResponse schema from Amazon CodeCatalyst
layout: schema
name: ListDevEnvironmentSessionsResponse
properties_list:
- description: ''
  name: items
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-list-dev-environment-sessions-response-schema.json
slug: amazon-codecatalyst-list-dev-environment-sessions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-dev-environment-sessions-response-schema.json\",\n  \"title\": \"ListDevEnvironmentSessionsResponse\",\n  \"description\": \"ListDevEnvironmentSessionsResponse schema from Amazon CodeCatalyst\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevEnvironmentSessionsSummaryList\"\n        },\n        {\n          \"description\": \"Information about each session retrieved in the list.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A token returned from a call to this API to indicate the next batch of results to return, if any.\"\n        }\n     \
  \ ]\n    }\n  },\n  \"required\": [\n    \"items\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-list-dev-environment-sessions-response-schema.json
tags:
- Amazon
- AWS
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: ListDevEnvironmentSessionsResponse
---
