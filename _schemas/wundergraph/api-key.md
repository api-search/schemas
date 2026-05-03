---
description: An API Key authenticates CLI and programmatic access to the WunderGraph Cosmo Platform API.
layout: schema
name: WunderGraph Cosmo API Key
properties_list:
- description: The name of the API key.
  name: name
  type: string
- description: When the key was created.
  name: createdAt
  type: string
- description: When the key expires.
  name: expiresAt
  type: string
- description: When the key was last used.
  name: lastUsedAt
  type: string
- description: Who created the key.
  name: createdBy
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/api-key.json
slug: api-key
source_filename: api-key.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/api-key.json\",\n  \"title\": \"WunderGraph Cosmo API Key\",\n  \"description\": \"An API Key authenticates CLI and programmatic access to the WunderGraph Cosmo Platform API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the API key.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the key was created.\"\n    },\n    \"expiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the key expires.\"\n    },\n    \"lastUsedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the key was last used.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Who created the key.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/api-key.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo API Key
---
