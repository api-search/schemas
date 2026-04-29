---
description: EmbeddedScopedTokenRequest schema from Airbyte API
layout: schema
name: EmbeddedScopedTokenRequest
properties_list:
- description: ''
  name: workspaceId
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-embedded-scoped-token-request-schema.json
slug: airbyte-embedded-scoped-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-scoped-token-request-schema.json\",\n  \"title\": \"EmbeddedScopedTokenRequest\",\n  \"description\": \"EmbeddedScopedTokenRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    }\n  },\n  \"required\": [\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-scoped-token-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EmbeddedScopedTokenRequest
---
