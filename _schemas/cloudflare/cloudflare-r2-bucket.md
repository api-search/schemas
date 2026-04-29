---
description: ''
layout: schema
name: Bucket
properties_list:
- description: The name of the bucket.
  name: name
  type: string
- description: When the bucket was created.
  name: creation_date
  type: string
- description: The location of the bucket.
  name: location
  type: string
- description: Default storage class for the bucket.
  name: storage_class
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-r2-bucket-schema.json
slug: cloudflare-r2-bucket
source_filename: cloudflare-r2-bucket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bucket\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the bucket.\"\n    },\n    \"creation_date\": {\n      \"type\": \"string\",\n      \"description\": \"When the bucket was created.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the bucket.\"\n    },\n    \"storage_class\": {\n      \"type\": \"string\",\n      \"description\": \"Default storage class for the bucket.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-r2-bucket-schema.json
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
title: Bucket
---
