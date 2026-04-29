---
description: UpdateWebhookRequest schema from AhaSend API
layout: schema
name: UpdateWebhookRequest
properties_list:
- description: Webhook name
  name: name
  type: string
- description: Webhook URL
  name: url
  type: string
- description: Whether the webhook is enabled
  name: enabled
  type: boolean
- description: Trigger on message reception
  name: on_reception
  type: boolean
- description: Trigger on message delivery
  name: on_delivered
  type: boolean
- description: Trigger on transient errors
  name: on_transient_error
  type: boolean
- description: Trigger on permanent failures
  name: on_failed
  type: boolean
- description: Trigger on bounces
  name: on_bounced
  type: boolean
- description: Trigger on suppressions
  name: on_suppressed
  type: boolean
- description: Trigger on opens
  name: on_opened
  type: boolean
- description: Trigger on clicks
  name: on_clicked
  type: boolean
- description: Trigger on suppression creation
  name: on_suppression_created
  type: boolean
- description: Trigger on DNS errors
  name: on_dns_error
  type: boolean
- description: Webhook scope
  name: scope
  type: string
- description: Domains this webhook applies to
  name: domains
  type: array
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-update-webhook-request-schema.json
slug: openapi-v2-update-webhook-request
source_filename: openapi-v2-update-webhook-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-webhook-request-schema.json\",\n  \"title\": \"UpdateWebhookRequest\",\n  \"description\": \"UpdateWebhookRequest schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"nullable\": true,\n      \"description\": \"Webhook name\",\n      \"example\": \"Example Name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"description\": \"Webhook URL\",\n      \"example\": \"https://example.com\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Whether the webhook is enabled\",\n      \"example\": true\n    },\n    \"on_reception\": {\n      \"type\": \"boolean\",\n      \"nullable\"\
  : true,\n      \"description\": \"Trigger on message reception\",\n      \"example\": true\n    },\n    \"on_delivered\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on message delivery\",\n      \"example\": true\n    },\n    \"on_transient_error\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on transient errors\",\n      \"example\": true\n    },\n    \"on_failed\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on permanent failures\",\n      \"example\": true\n    },\n    \"on_bounced\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on bounces\",\n      \"example\": true\n    },\n    \"on_suppressed\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on suppressions\",\n      \"example\": true\n    },\n    \"on_opened\": {\n      \"type\": \"boolean\"\
  ,\n      \"nullable\": true,\n      \"description\": \"Trigger on opens\",\n      \"example\": true\n    },\n    \"on_clicked\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on clicks\",\n      \"example\": true\n    },\n    \"on_suppression_created\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on suppression creation\",\n      \"example\": true\n    },\n    \"on_dns_error\": {\n      \"type\": \"boolean\",\n      \"nullable\": true,\n      \"description\": \"Trigger on DNS errors\",\n      \"example\": true\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Webhook scope\",\n      \"example\": \"example_value\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"nullable\": true,\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Domains this webhook applies to\",\n      \"example\": [\n\
  \        \"mail.example.com\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-update-webhook-request-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: UpdateWebhookRequest
---
