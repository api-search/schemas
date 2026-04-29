---
description: ResourceReference schema from Adyen API
layout: schema
name: ResourceReference
properties_list:
- description: The description of the resource.
  name: description
  type: string
- description: The unique identifier of the resource.
  name: id
  type: string
- description: The reference of the resource.
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-resource-reference-schema.json
slug: notification-webhooks-resource-reference
source_filename: notification-webhooks-resource-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-resource-reference-schema.json\",\n  \"title\": \"ResourceReference\",\n  \"description\": \"ResourceReference schema from Adyen API\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description of the resource.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the resource.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"The reference of the resource.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-resource-reference-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ResourceReference
---
