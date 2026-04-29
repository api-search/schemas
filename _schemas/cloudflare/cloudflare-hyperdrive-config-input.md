---
description: ''
layout: schema
name: ConfigInput
properties_list:
- description: Name for the configuration.
  name: name
  type: string
- description: ''
  name: origin
  type: object
- description: ''
  name: caching
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-hyperdrive-config-input-schema.json
slug: cloudflare-hyperdrive-config-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the configuration.\"\n    },\n    \"origin\": {\n      \"type\": \"object\"\n    },\n    \"caching\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-hyperdrive-config-input-schema.json
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
title: ConfigInput
---
