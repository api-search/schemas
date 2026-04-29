---
description: ''
layout: schema
name: Widget
properties_list:
- description: The public site key for the widget.
  name: sitekey
  type: string
- description: The secret key for server-side verification.
  name: secret
  type: string
- description: A human-readable name for the widget.
  name: name
  type: string
- description: Allowed domains for the widget.
  name: domains
  type: array
- description: The challenge mode for the widget.
  name: mode
  type: string
- description: Whether Bot Fight Mode is enabled.
  name: bot_fight_mode
  type: boolean
- description: ''
  name: created_on
  type: string
- description: ''
  name: modified_on
  type: string
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-turnstile-widget-schema.json
slug: cloudflare-turnstile-widget
source_filename: cloudflare-turnstile-widget-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Widget\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sitekey\": {\n      \"type\": \"string\",\n      \"description\": \"The public site key for the widget.\"\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"The secret key for server-side verification.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the widget.\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed domains for the widget.\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"The challenge mode for the widget.\"\n    },\n    \"bot_fight_mode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Bot Fight Mode is enabled.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\"\n    },\n    \"modified_on\": {\n      \"type\": \"string\"\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-turnstile-widget-schema.json
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
title: Widget
---
