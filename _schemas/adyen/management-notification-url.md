---
description: NotificationUrl schema from Adyen API
layout: schema
name: NotificationUrl
properties_list:
- description: One or more local URLs to send notifications to when using Terminal API.
  name: localUrls
  type: array
- description: One or more public URLs to send notifications to when using Terminal API.
  name: publicUrls
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-notification-url-schema.json
slug: management-notification-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-notification-url-schema.json\",\n  \"title\": \"NotificationUrl\",\n  \"description\": \"NotificationUrl schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"localUrls\": {\n      \"description\": \"One or more local URLs to send notifications to when using Terminal API.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Url\"\n      },\n      \"type\": \"array\"\n    },\n    \"publicUrls\": {\n      \"description\": \"One or more public URLs to send notifications to when using Terminal API.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Url\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-notification-url-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: NotificationUrl
---
