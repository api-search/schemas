---
description: WebhookEvent from GitLab API
layout: schema
name: WebhookEvent
properties_list:
- description: The unique identifier of the webhook event delivery.
  name: id
  type: integer
- description: The URL the event was delivered to.
  name: url
  type: string
- description: The event type that triggered the webhook delivery.
  name: trigger
  type: string
- description: HTTP headers sent with the webhook request.
  name: request_headers
  type: object
- description: The JSON payload body sent in the webhook request.
  name: request_data
  type: string
- description: HTTP headers returned in the webhook response.
  name: response_headers
  type: object
- description: The body of the response from the webhook receiver.
  name: response_body
  type: string
- description: The HTTP response status code returned by the receiver.
  name: response_status
  type: string
- description: Time in milliseconds the webhook delivery took.
  name: execution_duration
  type: number
- description: The date and time the event was delivered.
  name: created_at
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-webhooks-webhook-event-schema.json
slug: gitlab-webhooks-webhook-event
source_filename: gitlab-webhooks-webhook-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-event-schema.json\",\n  \"title\": \"WebhookEvent\",\n  \"description\": \"WebhookEvent from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the webhook event delivery.\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL the event was delivered to.\",\n      \"example\": \"https://gitlab.com/example\"\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"The event type that triggered the webhook delivery.\",\n      \"example\": \"example_value\"\n    },\n    \"request_headers\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP headers sent with the webhook\
  \ request.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"request_data\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON payload body sent in the webhook request.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"response_headers\": {\n      \"type\": \"object\",\n      \"description\": \"HTTP headers returned in the webhook response.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"response_body\": {\n      \"type\": \"string\",\n      \"description\": \"The body of the response from the webhook receiver.\",\n      \"example\": \"example_value\"\n    },\n    \"response_status\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP response status code returned by the receiver.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"execution_duration\": {\n      \"type\": \"number\",\n      \"description\": \"Time in milliseconds the webhook delivery\
  \ took.\",\n      \"example\": 42.5\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the event was delivered.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-webhooks-webhook-event-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: WebhookEvent
---
