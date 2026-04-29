---
description: ''
layout: schema
name: ProjectInput
properties_list:
- description: The name of the project.
  name: name
  type: string
- description: The production branch name.
  name: production_branch
  type: string
- description: ''
  name: build_config
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-pages-project-input-schema.json
slug: cloudflare-pages-project-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"production_branch\": {\n      \"type\": \"string\",\n      \"description\": \"The production branch name.\"\n    },\n    \"build_config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-pages-project-input-schema.json
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
title: ProjectInput
---
