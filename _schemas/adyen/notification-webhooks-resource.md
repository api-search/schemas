---
description: Resource schema from Adyen API
layout: schema
name: Resource
properties_list:
- description: Unique identifier of the balance platform.
  name: balancePlatform
  type: string
- description: Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.
  name: creationDate
  type: string
- description: The ID of the resource.
  name: id
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-resource-schema.json
slug: notification-webhooks-resource
source_filename: notification-webhooks-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-resource-schema.json\",\n  \"title\": \"Resource\",\n  \"description\": \"Resource schema from Adyen API\",\n  \"properties\": {\n    \"balancePlatform\": {\n      \"description\": \"Unique identifier of the balance platform.\",\n      \"type\": \"string\"\n    },\n    \"creationDate\": {\n      \"description\": \"Date and time when the event was triggered, in ISO 8601 extended format. For example, **2020-12-18T10:15:30+01:00**.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The ID of the resource.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-resource-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Resource
---
