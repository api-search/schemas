---
description: A Router Token authenticates a Cosmo Router instance with the WunderGraph Cosmo control plane.
layout: schema
name: WunderGraph Cosmo Router Token
properties_list:
- description: Unique identifier for the router token.
  name: id
  type: string
- description: The name of the router token.
  name: name
  type: string
- description: When the token was created.
  name: createdAt
  type: string
- description: When the token was last used.
  name: lastUsedAt
  type: string
provider_name: WunderGraph
provider_slug: wundergraph
schema_file: json-schema/router-token.json
slug: router-token
source_filename: router-token.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/wundergraph/blob/main/json-schema/router-token.json\",\n  \"title\": \"WunderGraph Cosmo Router Token\",\n  \"description\": \"A Router Token authenticates a Cosmo Router instance with the WunderGraph Cosmo control plane.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the router token.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the router token.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the token was created.\"\n    },\n    \"lastUsedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the token was last used.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/json-schema/router-token.json
tags:
- Federation
- GraphQL
- Management
- Schema Registry
title: WunderGraph Cosmo Router Token
---
