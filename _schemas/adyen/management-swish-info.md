---
description: SwishInfo schema from Adyen API
layout: schema
name: SwishInfo
properties_list:
- description: 'Swish number. Format: 10 digits without spaces. For example, **1231111111**.'
  name: swishNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-swish-info-schema.json
slug: management-swish-info
source_filename: management-swish-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-swish-info-schema.json\",\n  \"title\": \"SwishInfo\",\n  \"description\": \"SwishInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"swishNumber\": {\n      \"description\": \"Swish number. Format: 10 digits without spaces. For example, **1231111111**.\",\n      \"maxLength\": 10,\n      \"minLength\": 10,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"swishNumber\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-swish-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SwishInfo
---
