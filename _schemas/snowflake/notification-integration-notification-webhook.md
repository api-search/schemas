---
description: ''
layout: schema
name: NotificationWebhook
properties_list:
- description: The URL for the webhook. The URL must use the https:// protocol.
  name: webhook_url
  type: string
- description: A template for the body of the HTTP request to send for the notification.
  name: webhook_body_template
  type: string
- description: A list of HTTP headers and values to include in the HTTP request for the webhook.
  name: webhook_headers
  type: object
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-webhook-schema.json
slug: notification-integration-notification-webhook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationWebhook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"webhook_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL for the webhook. The URL must use the https:// protocol.\"\n    },\n    \"webhook_body_template\": {\n      \"type\": \"string\",\n      \"description\": \"A template for the body of the HTTP request to send for the notification.\"\n    },\n    \"webhook_headers\": {\n      \"type\": \"object\",\n      \"description\": \"A list of HTTP headers and values to include in the HTTP request for the webhook.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-webhook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationWebhook
---
