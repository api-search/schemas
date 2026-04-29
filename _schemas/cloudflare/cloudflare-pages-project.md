---
description: ''
layout: schema
name: Project
properties_list:
- description: The unique identifier of the project.
  name: id
  type: string
- description: The name of the project.
  name: name
  type: string
- description: The subdomain for the project.
  name: subdomain
  type: string
- description: Custom domains attached to the project.
  name: domains
  type: array
- description: The production branch name.
  name: production_branch
  type: string
- description: When the project was created.
  name: created_on
  type: string
- description: ''
  name: build_config
  type: object
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-pages-project-schema.json
slug: cloudflare-pages-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"subdomain\": {\n      \"type\": \"string\",\n      \"description\": \"The subdomain for the project.\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"Custom domains attached to the project.\"\n    },\n    \"production_branch\": {\n      \"type\": \"string\",\n      \"description\": \"The production branch name.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"When the project was created.\"\n    },\n    \"build_config\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-pages-project-schema.json
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
title: Project
---
