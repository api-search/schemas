---
description: ''
layout: schema
name: NotificationHook
properties_list:
- description: Type of NotificationHook, can be QUEUE, EMAIL or WEBHOOK
  name: type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/notification-integration-notification-hook-schema.json
slug: notification-integration-notification-hook
source_filename: notification-integration-notification-hook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotificationHook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of NotificationHook, can be QUEUE, EMAIL or WEBHOOK\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/notification-integration-notification-hook-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: NotificationHook
---
