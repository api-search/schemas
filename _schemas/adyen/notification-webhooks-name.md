---
description: Name schema from Adyen API
layout: schema
name: Name
properties_list:
- description: The first name.
  name: firstName
  type: string
- description: The last name.
  name: lastName
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-name-schema.json
slug: notification-webhooks-name
source_filename: notification-webhooks-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"Name schema from Adyen API\",\n  \"properties\": {\n    \"firstName\": {\n      \"description\": \"The first name.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The last name.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\"\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-name-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Name
---
