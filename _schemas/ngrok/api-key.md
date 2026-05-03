---
description: An API Key is used to authenticate requests to the ngrok API.
layout: schema
name: ngrok API Key
properties_list:
- description: Unique identifier for the API key.
  name: id
  type: string
- description: URI of the API key resource.
  name: uri
  type: string
- description: Human-readable description of the API key.
  name: description
  type: string
- description: Arbitrary user-defined metadata.
  name: metadata
  type: string
- description: Timestamp when the API key was created.
  name: created_at
  type: string
- description: The API key token. Only present in the response to a create request.
  name: token
  type: string
- description: The owner of the API key, if owned by a bot user.
  name: owner_id
  type: string
provider_name: ngrok
provider_slug: ngrok
schema_file: json-schema/api-key.json
slug: api-key
source_filename: api-key.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/ngrok/blob/main/json-schema/api-key.json\",\n  \"title\": \"ngrok API Key\",\n  \"description\": \"An API Key is used to authenticate requests to the ngrok API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API key.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI of the API key resource.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the API key.\"\n    },\n    \"metadata\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary user-defined metadata.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the API key was created.\"\n    },\n    \"token\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"The API key token. Only present in the response to a create request.\"\n    },\n    \"owner_id\": {\n      \"type\": \"string\",\n      \"description\": \"The owner of the API key, if owned by a bot user.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/json-schema/api-key.json
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
title: ngrok API Key
---
