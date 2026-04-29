---
description: ''
layout: schema
name: Namespace
properties_list:
- description: The unique identifier of the namespace.
  name: id
  type: string
- description: The human-readable title of the namespace.
  name: title
  type: string
- description: Whether the namespace supports URL-encoded keys.
  name: supports_url_encoding
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-kv-namespace-schema.json
slug: cloudflare-kv-namespace
source_filename: cloudflare-kv-namespace-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Namespace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the namespace.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable title of the namespace.\"\n    },\n    \"supports_url_encoding\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the namespace supports URL-encoded keys.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-kv-namespace-schema.json
tags:
- AI Gateway
- API Gateway
- Artificial Intelligence
- CDN
- Cloud
- Containers
- DDoS Protection
- DNS
- Edge
- Edge Computing
- Object Storage
- Platform
- Real-Time Communication
- Security
- Serverless
- Web Performance
title: Namespace
---
