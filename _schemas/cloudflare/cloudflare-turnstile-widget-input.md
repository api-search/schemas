---
description: ''
layout: schema
name: WidgetInput
properties_list:
- description: Name for the widget.
  name: name
  type: string
- description: Allowed domains.
  name: domains
  type: array
- description: ''
  name: mode
  type: string
- description: ''
  name: bot_fight_mode
  type: boolean
provider_name: Cloudflare
provider_slug: cloudflare
schema_file: json-schema/cloudflare-turnstile-widget-input-schema.json
slug: cloudflare-turnstile-widget-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WidgetInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the widget.\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"Allowed domains.\"\n    },\n    \"mode\": {\n      \"type\": \"string\"\n    },\n    \"bot_fight_mode\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudflare/refs/heads/main/json-schema/cloudflare-turnstile-widget-input-schema.json
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
title: WidgetInput
---
