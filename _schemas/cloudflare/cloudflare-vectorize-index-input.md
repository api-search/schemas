---
description: ''
layout: schema
name: IndexInput
properties_list:
- description: The name of the index.
  name: name
  type: string
- description: Description of the index.
  name: description
  type: string
- description: ''
  name: config
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-vectorize-index-input-schema.json
slug: cloudflare-vectorize-index-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndexInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the index.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the index.\"\n    },\n    \"config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-vectorize-index-input-schema.json
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
title: IndexInput
---
