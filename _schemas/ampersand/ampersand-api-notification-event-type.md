---
description: The type of notification event.
layout: schema
name: NotificationEventType
properties_list: []
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-notification-event-type-schema.json
slug: ampersand-api-notification-event-type
source_filename: ampersand-api-notification-event-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-notification-event-type-schema.json\",\n  \"title\": \"NotificationEventType\",\n  \"description\": \"The type of notification event.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"connection.created\",\n    \"connection.error\",\n    \"connection.refreshed\",\n    \"connection.deleted\",\n    \"installation.created\",\n    \"installation.updated\",\n    \"installation.deleted\",\n    \"read.schedule.paused\",\n    \"read.backfill.done\",\n    \"read.triggered.done\",\n    \"read.triggered.error\",\n    \"write.async.done\",\n    \"destination.webhook.disabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-notification-event-type-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: NotificationEventType
---
