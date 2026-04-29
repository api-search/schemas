---
description: Expiry schema from Adyen API
layout: schema
name: Expiry
properties_list:
- description: The month in which the card will expire.
  name: month
  type: string
- description: The year in which the card will expire.
  name: year
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-expiry-schema.json
slug: notification-webhooks-expiry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-expiry-schema.json\",\n  \"title\": \"Expiry\",\n  \"description\": \"Expiry schema from Adyen API\",\n  \"properties\": {\n    \"month\": {\n      \"description\": \"The month in which the card will expire.\",\n      \"type\": \"string\"\n    },\n    \"year\": {\n      \"description\": \"The year in which the card will expire.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-expiry-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Expiry
---
