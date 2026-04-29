---
description: A D1 serverless SQL database object from the Cloudflare API, representing an SQLite-compatible database running on Cloudflare's global network with support for time travel and automatic replication.
layout: schema
name: Cloudflare D1 Database
properties_list:
- description: The unique identifier of the D1 database.
  name: uuid
  type: string
- description: The name of the database.
  name: name
  type: string
- description: The internal version of the database.
  name: version
  type: string
- description: The number of tables in the database.
  name: num_tables
  type: integer
- description: The size of the database file in bytes.
  name: file_size
  type: integer
- description: The region where the primary database is running.
  name: running_in_region
  type: string
- description: When the database was created.
  name: created_at
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-d1-database-schema.json
slug: cloudflare-d1-database
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-d1-database-schema.json\",\n  \"title\": \"Cloudflare D1 Database\",\n  \"description\": \"A D1 serverless SQL database object from the Cloudflare API, representing an SQLite-compatible database running on Cloudflare's global network with support for time travel and automatic replication.\",\n  \"type\": \"object\",\n  \"required\": [\"uuid\", \"name\"],\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the D1 database.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the database.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The internal version of the database.\"\n    },\n    \"num_tables\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The number of tables in the database.\",\n      \"minimum\": 0\n    },\n    \"file_size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the database file in bytes.\",\n      \"minimum\": 0\n    },\n    \"running_in_region\": {\n      \"type\": \"string\",\n      \"description\": \"The region where the primary database is running.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the database was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-d1-database-schema.json
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
title: Cloudflare D1 Database
---
