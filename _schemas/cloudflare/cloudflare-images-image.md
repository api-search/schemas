---
description: ''
layout: schema
name: Image
properties_list:
- description: The unique identifier of the image.
  name: id
  type: string
- description: Original filename.
  name: filename
  type: string
- description: User-defined metadata.
  name: metadata
  type: object
- description: Upload timestamp.
  name: uploaded
  type: string
- description: ''
  name: requireSignedURLs
  type: boolean
- description: URLs for each variant of the image.
  name: variants
  type: array
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-images-image-schema.json
slug: cloudflare-images-image
source_filename: cloudflare-images-image-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Image\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the image.\"\n    },\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Original filename.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined metadata.\"\n    },\n    \"uploaded\": {\n      \"type\": \"string\",\n      \"description\": \"Upload timestamp.\"\n    },\n    \"requireSignedURLs\": {\n      \"type\": \"boolean\"\n    },\n    \"variants\": {\n      \"type\": \"array\",\n      \"description\": \"URLs for each variant of the image.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-images-image-schema.json
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
title: Image
---
