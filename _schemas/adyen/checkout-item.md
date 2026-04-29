---
description: Item schema from Adyen API
layout: schema
name: Item
properties_list:
- description: The value to provide in the result.
  name: id
  type: string
- description: The display name.
  name: name
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-item-schema.json
slug: checkout-item
source_filename: checkout-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-item-schema.json\",\n  \"title\": \"Item\",\n  \"description\": \"Item schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The value to provide in the result.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The display name.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-item-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Item
---
