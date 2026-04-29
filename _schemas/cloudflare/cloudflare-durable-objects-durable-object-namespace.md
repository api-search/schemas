---
description: ''
layout: schema
name: DurableObjectNamespace
properties_list:
- description: The unique identifier of the namespace.
  name: id
  type: string
- description: The name of the namespace.
  name: name
  type: string
- description: The Worker script associated with the namespace.
  name: script
  type: string
- description: The Durable Object class name.
  name: class
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-durable-objects-durable-object-namespace-schema.json
slug: cloudflare-durable-objects-durable-object-namespace
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DurableObjectNamespace\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the namespace.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the namespace.\"\n    },\n    \"script\": {\n      \"type\": \"string\",\n      \"description\": \"The Worker script associated with the namespace.\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"The Durable Object class name.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-durable-objects-durable-object-namespace-schema.json
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
title: DurableObjectNamespace
---
