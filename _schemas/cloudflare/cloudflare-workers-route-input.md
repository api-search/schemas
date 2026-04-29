---
description: ''
layout: schema
name: RouteInput
properties_list:
- description: The URL pattern for the route, e.g. example.com/*.
  name: pattern
  type: string
- description: The name of the Worker script to invoke.
  name: script
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-workers-route-input-schema.json
slug: cloudflare-workers-route-input
source_filename: cloudflare-workers-route-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RouteInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pattern\": {\n      \"type\": \"string\",\n      \"description\": \"The URL pattern for the route, e.g. example.com/*.\"\n    },\n    \"script\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Worker script to invoke.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-workers-route-input-schema.json
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
title: RouteInput
---
