---
description: ''
layout: schema
name: VerifyResponse
properties_list:
- description: Whether the token was valid.
  name: success
  type: boolean
- description: Timestamp of the challenge.
  name: challenge_ts
  type: string
- description: Hostname for which the challenge was solved.
  name: hostname
  type: string
- description: Error codes if verification failed.
  name: error-codes
  type: array
- description: The action name from the widget.
  name: action
  type: string
- description: Custom data from the widget.
  name: cdata
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-turnstile-verify-response-schema.json
slug: cloudflare-turnstile-verify-response
source_filename: cloudflare-turnstile-verify-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VerifyResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the token was valid.\"\n    },\n    \"challenge_ts\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the challenge.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname for which the challenge was solved.\"\n    },\n    \"error-codes\": {\n      \"type\": \"array\",\n      \"description\": \"Error codes if verification failed.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action name from the widget.\"\n    },\n    \"cdata\": {\n      \"type\": \"string\",\n      \"description\": \"Custom data from the widget.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-turnstile-verify-response-schema.json
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
title: VerifyResponse
---
