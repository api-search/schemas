---
description: ''
layout: schema
name: MessageInput
properties_list:
- description: The message body content.
  name: body
  type: string
- description: The content type of the message body.
  name: content_type
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-queues-message-input-schema.json
slug: cloudflare-queues-message-input
source_filename: cloudflare-queues-message-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MessageInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"The message body content.\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the message body.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-queues-message-input-schema.json
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
title: MessageInput
---
