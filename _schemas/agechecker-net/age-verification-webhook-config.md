---
description: WebhookConfig schema from AgeChecker.Net API
layout: schema
name: WebhookConfig
properties_list:
- description: Webhook configuration identifier.
  name: id
  type: string
- description: URL to receive webhook events.
  name: url
  type: string
- description: List of event types to receive.
  name: events
  type: array
- description: Shared secret for webhook signature verification.
  name: secret
  type: string
- description: When the webhook was configured.
  name: created_at
  type: string
provider_name: AgeChecker.Net
provider_slug: agechecker-net
schema_file: json-schema/age-verification-webhook-config-schema.json
slug: age-verification-webhook-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-webhook-config-schema.json\",\n  \"title\": \"WebhookConfig\",\n  \"description\": \"WebhookConfig schema from AgeChecker.Net API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook configuration identifier.\",\n      \"example\": \"500123\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to receive webhook events.\",\n      \"example\": \"https://example.com\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of event types to receive.\",\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"secret\": {\n      \"type\": \"string\",\n      \"description\": \"Shared\
  \ secret for webhook signature verification.\",\n      \"example\": \"example_value\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the webhook was configured.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agechecker-net/refs/heads/main/json-schema/age-verification-webhook-config-schema.json
tags:
- Age Verification
- Identity
- Compliance
- Regulatory
- E-Commerce
title: WebhookConfig
---
