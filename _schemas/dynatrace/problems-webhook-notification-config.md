---
description: Configuration for a webhook notification integration in Dynatrace. Posted to POST /api/config/v1/notifications to register the webhook.
layout: schema
name: WebhookNotificationConfig
properties_list:
- description: The notification type. Must be WEBHOOK for webhook integrations.
  name: type
  type: string
- description: A display name for this notification configuration.
  name: name
  type: string
- description: Whether this notification integration is active.
  name: active
  type: boolean
- description: The HTTPS URL of the webhook endpoint that will receive problem notifications.
  name: url
  type: string
- description: The ID of the alerting profile (problem filter) that controls which problems trigger this notification.
  name: alertingProfile
  type: string
- description: Optional HTTP headers to include in the webhook request, such as authorization headers or content-type overrides.
  name: headers
  type: array
- description: Whether to accept any TLS certificate from the webhook endpoint. Should be false in production environments.
  name: acceptAnyCertificate
  type: boolean
- description: The custom payload template using Dynatrace placeholder variables such as {ProblemID}, {ProblemTitle}, {State}. If not specified, Dynatrace uses the default JSON payload format.
  name: payload
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-webhook-notification-config-schema.json
slug: problems-webhook-notification-config
source_filename: problems-webhook-notification-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-webhook-notification-config-schema.json\",\n  \"title\": \"WebhookNotificationConfig\",\n  \"description\": \"Configuration for a webhook notification integration in Dynatrace. Posted to POST /api/config/v1/notifications to register the webhook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The notification type. Must be WEBHOOK for webhook integrations.\",\n      \"enum\": [\n        \"WEBHOOK\"\n      ],\n      \"example\": \"WEBHOOK\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A display name for this notification configuration.\",\n      \"example\": \"My Problem Webhook\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this notification integration\
  \ is active.\",\n      \"example\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The HTTPS URL of the webhook endpoint that will receive problem notifications.\",\n      \"example\": \"https://webhook.example.com/webhook/dynatrace/problems\"\n    },\n    \"alertingProfile\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the alerting profile (problem filter) that controls which problems trigger this notification.\",\n      \"example\": \"alerting-profile-uuid\"\n    },\n    \"headers\": {\n      \"type\": \"array\",\n      \"description\": \"Optional HTTP headers to include in the webhook request, such as authorization headers or content-type overrides.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WebhookHeader\"\n      },\n      \"example\": [\n        {\n          \"name\": \"Authorization\",\n          \"value\": \"Bearer my-secret-token\"\n        }\n      ]\n    },\n    \"acceptAnyCertificate\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to accept any TLS certificate from the webhook endpoint. Should be false in production environments.\",\n      \"example\": false\n    },\n    \"payload\": {\n      \"type\": \"string\",\n      \"description\": \"The custom payload template using Dynatrace placeholder variables such as {ProblemID}, {ProblemTitle}, {State}. If not specified, Dynatrace uses the default JSON payload format.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"name\",\n    \"active\",\n    \"url\",\n    \"alertingProfile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-webhook-notification-config-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: WebhookNotificationConfig
---
