---
description: Webhook schema from AhaSend API
layout: schema
name: Webhook
properties_list:
- description: Object type identifier
  name: object
  type: string
- description: Unique identifier for the webhook
  name: id
  type: string
- description: When the webhook was created
  name: created_at
  type: string
- description: When the webhook was last updated
  name: updated_at
  type: string
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
- description: Number of successful calls
  name: success_count
  type: integer
- description: Number of unsuccessful calls
  name: error_count
  type: integer
- description: Number of consecutive failed calls
  name: errors_since_last_success
  type: integer
- description: When the webhook was last called
  name: last_request_at
  type: string
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-webhook-schema.json
slug: openapi-v2-webhook
source_filename: openapi-v2-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-webhook-schema.json\",\n  \"title\": \"Webhook\",\n  \"description\": \"Webhook schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"webhook\"\n      ],\n      \"description\": \"Object type identifier\",\n      \"example\": \"webhook\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the webhook\",\n      \"example\": \"500123\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the webhook was created\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"\
  description\": \"When the webhook was last updated\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Webhook name\",\n      \"example\": \"Example Name\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL\",\n      \"example\": \"https://example.com\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the webhook is enabled\",\n      \"example\": true\n    },\n    \"on_reception\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on message reception\",\n      \"example\": true\n    },\n    \"on_delivered\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on message delivery\",\n      \"example\": true\n    },\n    \"on_transient_error\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on transient errors\",\n      \"example\": true\n    },\n    \"on_failed\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on permanent failures\",\n      \"example\": true\n    },\n    \"on_bounced\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on bounces\",\n      \"example\": true\n    },\n    \"on_suppressed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on suppressions\",\n      \"example\": true\n    },\n    \"on_opened\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on opens\",\n      \"example\": true\n    },\n    \"on_clicked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on clicks\",\n      \"example\": true\n    },\n    \"on_suppression_created\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on suppression creation\",\n      \"example\": true\n    },\n    \"on_dns_error\": {\n      \"type\": \"boolean\",\n      \"description\": \"Trigger on DNS errors\",\n      \"example\": true\n    },\n    \"scope\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Webhook scope\",\n      \"example\": \"example_value\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Domains this webhook applies to\",\n      \"example\": [\n        \"mail.example.com\"\n      ]\n    },\n    \"success_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of successful calls\",\n      \"example\": 1\n    },\n    \"error_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of unsuccessful calls\",\n      \"example\": 1\n    },\n    \"errors_since_last_success\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of consecutive failed calls\",\n      \"example\": 1\n    },\n    \"last_request_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the webhook was last called\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"\
  required\": [\n    \"object\",\n    \"id\",\n    \"created_at\",\n    \"updated_at\",\n    \"name\",\n    \"url\",\n    \"enabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-webhook-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Webhook
---
