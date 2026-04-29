---
description: JSONObject schema from Adyen API
layout: schema
name: JSONObject
properties_list:
- description: ''
  name: paths
  type: array
- description: ''
  name: rootPath
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-json-object-schema.json
slug: notification-webhooks-json-object
source_filename: notification-webhooks-json-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-json-object-schema.json\",\n  \"title\": \"JSONObject\",\n  \"description\": \"JSONObject schema from Adyen API\",\n  \"properties\": {\n    \"paths\": {\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JSONPath\"\n      },\n      \"type\": \"array\"\n    },\n    \"rootPath\": {\n      \"$ref\": \"#/components/schemas/JSONPath\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-json-object-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: JSONObject
---
