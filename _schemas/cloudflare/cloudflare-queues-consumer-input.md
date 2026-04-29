---
description: ''
layout: schema
name: ConsumerInput
properties_list:
- description: The Worker script name that will consume messages.
  name: script_name
  type: string
- description: ''
  name: settings
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-queues-consumer-input-schema.json
slug: cloudflare-queues-consumer-input
source_filename: cloudflare-queues-consumer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConsumerInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"script_name\": {\n      \"type\": \"string\",\n      \"description\": \"The Worker script name that will consume messages.\"\n    },\n    \"settings\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-queues-consumer-input-schema.json
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
title: ConsumerInput
---
