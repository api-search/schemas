---
description: Config schema from Ampersand API
layout: schema
name: Config
properties_list:
- description: The config ID.
  name: id
  type: string
- description: The ID of the revision that was current when this config was created or last updated.
  name: revisionId
  type: string
- description: The time the config was created.
  name: createTime
  type: string
- description: The person who created the config, in the format of "consumer:{consumer-id}" or "builder:{builder-id}".
  name: createdBy
  type: string
- description: ''
  name: content
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-config-schema.json
slug: ampersand-api-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-config-schema.json\",\n  \"title\": \"Config\",\n  \"description\": \"Config schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The config ID.\",\n      \"example\": \"config-123\"\n    },\n    \"revisionId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the revision that was current when this config was created or last updated. \\n\",\n      \"example\": \"revision-123\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time the config was created.\",\n      \"format\": \"date-time\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"The person who created the config, in the format of \\\"consumer:{consumer-id}\\\
  \" or \\\"builder:{builder-id}\\\".\",\n      \"example\": \"builder:builder-123\"\n    },\n    \"content\": {\n      \"$ref\": \"../config/config.yaml#/components/schemas/ConfigContent\"\n    }\n  },\n  \"required\": [\n    \"content\",\n    \"createTime\",\n    \"createdBy\",\n    \"id\",\n    \"revisionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-config-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Config
---
