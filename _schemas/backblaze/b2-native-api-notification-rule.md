---
description: NotificationRule schema from Backblaze B2 Native API
layout: schema
name: NotificationRule
properties_list:
- description: Name for this notification rule
  name: name
  type: string
- description: Event types that trigger this notification
  name: eventTypes
  type: array
- description: Whether this rule is enabled
  name: isEnabled
  type: boolean
- description: ''
  name: targetConfiguration
  type: object
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-notification-rule-schema.json
slug: b2-native-api-notification-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-notification-rule-schema.json\",\n  \"title\": \"NotificationRule\",\n  \"description\": \"NotificationRule schema from Backblaze B2 Native API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for this notification rule\",\n      \"example\": \"my-notification\"\n    },\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Event types that trigger this notification\",\n      \"example\": [\n        \"b2:ObjectCreated:Upload\"\n      ]\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this rule is enabled\",\n      \"example\": true\n    },\n    \"targetConfiguration\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"targetType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"url\"\n          ],\n          \"description\": \"Type of notification target\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Webhook URL to send notifications to\",\n          \"example\": \"https://my-app.example.com/webhooks/b2\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/json-schema/b2-native-api-notification-rule-schema.json
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: NotificationRule
---
