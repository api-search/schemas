---
description: ''
layout: schema
name: D1Database
properties_list:
- description: The unique identifier of the database.
  name: uuid
  type: string
- description: The name of the database.
  name: name
  type: string
- description: The version of the database.
  name: version
  type: string
- description: Number of tables in the database.
  name: num_tables
  type: integer
- description: Size of the database file in bytes.
  name: file_size
  type: integer
- description: When the database was created.
  name: created_at
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-d1-d1-database-schema.json
slug: cloudflare-d1-d1-database
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"D1Database\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the database.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the database.\"\n    },\n    \"num_tables\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of tables in the database.\"\n    },\n    \"file_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the database file in bytes.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the database was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-d1-d1-database-schema.json
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
title: D1Database
---
