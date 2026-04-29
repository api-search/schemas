---
description: ''
layout: schema
name: WorkerInput
properties_list:
- description: The name of the Worker.
  name: name
  type: string
- description: The entry point module for the Worker.
  name: main_module
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-workers-worker-input-schema.json
slug: cloudflare-workers-worker-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkerInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Worker.\"\n    },\n    \"main_module\": {\n      \"type\": \"string\",\n      \"description\": \"The entry point module for the Worker.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-workers-worker-input-schema.json
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
title: WorkerInput
---
