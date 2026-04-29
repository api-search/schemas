---
description: Configures a notification.
layout: schema
name: NotificationConfig
properties_list:
- description: ''
  name: email
  type: object
- description: ''
  name: webhook
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-notification-config-schema.json
slug: airbyte-notification-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-notification-config-schema.json\",\n  \"title\": \"NotificationConfig\",\n  \"description\": \"Configures a notification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"$ref\": \"#/components/schemas/EmailNotificationConfig\"\n    },\n    \"webhook\": {\n      \"$ref\": \"#/components/schemas/WebhookNotificationConfig\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-notification-config-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: NotificationConfig
---
