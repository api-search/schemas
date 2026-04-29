---
description: ''
layout: schema
name: Node
properties_list:
- description: ''
  name: node_id
  type: string
- description: ''
  name: api_key
  type: string
- description: ''
  name: group_id
  type: string
- description: ''
  name: node_version
  type: string
- description: ''
  name: ttl
  type: integer
- description: ''
  name: tags
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-mdcb-node-schema.json
slug: tyk-mdcb-node
source_filename: tyk-mdcb-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Node\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"node_id\": {\n      \"type\": \"string\"\n    },\n    \"api_key\": {\n      \"type\": \"string\"\n    },\n    \"group_id\": {\n      \"type\": \"string\"\n    },\n    \"node_version\": {\n      \"type\": \"string\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-mdcb-node-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: Node
---
