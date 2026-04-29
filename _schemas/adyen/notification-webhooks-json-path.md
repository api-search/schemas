---
description: JSONPath schema from Adyen API
layout: schema
name: JSONPath
properties_list:
- description: ''
  name: content
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-json-path-schema.json
slug: notification-webhooks-json-path
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-json-path-schema.json\",\n  \"title\": \"JSONPath\",\n  \"description\": \"JSONPath schema from Adyen API\",\n  \"properties\": {\n    \"content\": {\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-json-path-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: JSONPath
---
