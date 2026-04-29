---
description: Additional headers to add when Ampersand sends a webhook message
layout: schema
name: WebhookHeaders
properties_list: []
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-webhook-headers-schema.json
slug: ampersand-api-webhook-headers
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-webhook-headers-schema.json\",\n  \"title\": \"WebhookHeaders\",\n  \"description\": \"Additional headers to add when Ampersand sends a webhook message\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"string\",\n    \"nullable\": false\n  },\n  \"example\": {\n    \"Authorization\": \"Bearer 1234\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-webhook-headers-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: WebhookHeaders
---
