---
description: ''
layout: schema
name: Deployment
properties_list:
- description: The unique identifier of the deployment.
  name: id
  type: string
- description: The URL of the deployment.
  name: url
  type: string
- description: The deployment environment.
  name: environment
  type: string
- description: When the deployment was created.
  name: created_on
  type: string
- description: ''
  name: latest_stage
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-pages-deployment-schema.json
slug: cloudflare-pages-deployment
source_filename: cloudflare-pages-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the deployment.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the deployment.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment environment.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the deployment was created.\"\n    },\n    \"latest_stage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-pages-deployment-schema.json
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
title: Deployment
---
