---
description: ''
layout: schema
name: GraphQLSupergraphConfig
properties_list:
- description: ''
  name: disable_query_batching
  type: boolean
- description: ''
  name: global_headers
  type: object
- description: ''
  name: merged_sdl
  type: string
- description: ''
  name: subgraphs
  type: array
- description: ''
  name: updated_at
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-graph-ql-supergraph-config-schema.json
slug: tyk-gateway-graph-ql-supergraph-config
source_filename: tyk-gateway-graph-ql-supergraph-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GraphQLSupergraphConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disable_query_batching\": {\n      \"type\": \"boolean\"\n    },\n    \"global_headers\": {\n      \"type\": \"object\"\n    },\n    \"merged_sdl\": {\n      \"type\": \"string\"\n    },\n    \"subgraphs\": {\n      \"type\": \"array\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-graph-ql-supergraph-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: GraphQLSupergraphConfig
---
