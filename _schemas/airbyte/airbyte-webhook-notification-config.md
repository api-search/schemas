---
description: Configures a webhook notification.
layout: schema
name: WebhookNotificationConfig
properties_list:
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: url
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-webhook-notification-config-schema.json
slug: airbyte-webhook-notification-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-webhook-notification-config-schema.json\",\n  \"title\": \"WebhookNotificationConfig\",\n  \"description\": \"Configures a webhook notification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-webhook-notification-config-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: WebhookNotificationConfig
---
