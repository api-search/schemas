---
description: Nexo schema from Adyen API
layout: schema
name: Nexo
properties_list:
- description: The list of local and public URLs to send display notifications to when using Terminal API.
  name: displayUrls
  type: object
- description: The key you share with Adyen to secure local communications when using Terminal API.
  name: encryptionKey
  type: object
- description: The list of local and public URLs to send event notifications to when using Terminal API.
  name: eventUrls
  type: object
- description: One or more URLs to send event messages to when using Terminal API.
  name: nexoEventUrls
  type: array
- description: Configures sending event notifications by pressing a button on a terminal, for example used for pay-at-table.
  name: notification
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-nexo-schema.json
slug: management-nexo
source_filename: management-nexo-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-nexo-schema.json\",\n  \"title\": \"Nexo\",\n  \"description\": \"Nexo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"displayUrls\": {\n      \"description\": \"The list of local and public URLs to send display notifications to when using Terminal API.\",\n      \"$ref\": \"#/components/schemas/NotificationUrl\"\n    },\n    \"encryptionKey\": {\n      \"description\": \"The key you share with Adyen to secure local communications when using Terminal API.\",\n      \"$ref\": \"#/components/schemas/Key\"\n    },\n    \"eventUrls\": {\n      \"description\": \"The list of local and public URLs to send event notifications to when using Terminal API.\",\n      \"$ref\": \"#/components/schemas/EventUrl\"\n    },\n    \"nexoEventUrls\": {\n      \"deprecated\": true,\n      \"\
  x-deprecatedInVersion\": \"1\",\n      \"x-deprecatedMessage\": \"Use `eventUrls` instead.\",\n      \"description\": \"One or more URLs to send event messages to when using Terminal API.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"notification\": {\n      \"description\": \"Configures sending event notifications by pressing a button on a terminal, for example used for pay-at-table.\",\n      \"$ref\": \"#/components/schemas/Notification\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-nexo-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Nexo
---
