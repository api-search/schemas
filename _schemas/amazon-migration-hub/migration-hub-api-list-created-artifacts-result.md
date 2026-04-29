---
description: ListCreatedArtifactsResult schema from Amazon Migration Hub API
layout: schema
name: ListCreatedArtifactsResult
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: CreatedArtifactList
  type: object
provider_name: Amazon Migration Hub
provider_slug: amazon-migration-hub
schema_file: json-schema/migration-hub-api-list-created-artifacts-result-schema.json
slug: migration-hub-api-list-created-artifacts-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-created-artifacts-result-schema.json\",\n  \"title\": \"ListCreatedArtifactsResult\",\n  \"description\": \"ListCreatedArtifactsResult schema from Amazon Migration Hub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Token\"\n        },\n        {\n          \"description\": \"If there are more created artifacts than the max result, return the next token to be passed to the next call as a bookmark of where to start from.\"\n        }\n      ]\n    },\n    \"CreatedArtifactList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreatedArtifactList\"\n        },\n        {\n          \"description\": \"List of created artifacts up to the maximum number\
  \ of results specified in the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-migration-hub/refs/heads/main/json-schema/migration-hub-api-list-created-artifacts-result-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListCreatedArtifactsResult
---
