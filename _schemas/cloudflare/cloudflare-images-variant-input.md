---
description: ''
layout: schema
name: VariantInput
properties_list:
- description: The name of the variant.
  name: id
  type: string
- description: ''
  name: options
  type: object
- description: Allow unsigned URL access for this variant.
  name: neverRequireSignedURLs
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-images-variant-input-schema.json
slug: cloudflare-images-variant-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VariantInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the variant.\"\n    },\n    \"options\": {\n      \"type\": \"object\"\n    },\n    \"neverRequireSignedURLs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Allow unsigned URL access for this variant.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-images-variant-input-schema.json
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
title: VariantInput
---
