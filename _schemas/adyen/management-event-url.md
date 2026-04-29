---
description: EventUrl schema from Adyen API
layout: schema
name: EventUrl
properties_list:
- description: One or more local URLs to send event notifications to when using Terminal API.
  name: eventLocalUrls
  type: array
- description: One or more public URLs to send event notifications to when using Terminal API.
  name: eventPublicUrls
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-event-url-schema.json
slug: management-event-url
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-event-url-schema.json\",\n  \"title\": \"EventUrl\",\n  \"description\": \"EventUrl schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventLocalUrls\": {\n      \"description\": \"One or more local URLs to send event notifications to when using Terminal API.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Url\"\n      },\n      \"type\": \"array\"\n    },\n    \"eventPublicUrls\": {\n      \"description\": \"One or more public URLs to send event notifications to when using Terminal API.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Url\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-event-url-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: EventUrl
---
