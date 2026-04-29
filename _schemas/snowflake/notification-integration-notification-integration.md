---
description: A Snowflake notification
layout: schema
name: NotificationIntegration
properties_list:
- description: Name of the notification.
  name: name
  type: string
- description: Whether the notification integration is enabled.
  name: enabled
  type: boolean
- description: Comment for the notification integration.
  name: comment
  type: string
- description: Date and time when the notification was created.
  name: created_on
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-integration-schema.json
slug: notification-integration-notification-integration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationIntegration\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake notification\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the notification.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the notification integration is enabled.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Comment for the notification integration.\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the notification was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-integration-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationIntegration
---
