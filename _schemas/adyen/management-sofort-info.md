---
description: SofortInfo schema from Adyen API
layout: schema
name: SofortInfo
properties_list:
- description: Sofort currency code. For example, **EUR**.
  name: currencyCode
  type: string
- description: 'Sofort logo. Format: Base64-encoded string.'
  name: logo
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-sofort-info-schema.json
slug: management-sofort-info
source_filename: management-sofort-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-sofort-info-schema.json\",\n  \"title\": \"SofortInfo\",\n  \"description\": \"SofortInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"description\": \"Sofort currency code. For example, **EUR**.\",\n      \"type\": \"string\"\n    },\n    \"logo\": {\n      \"description\": \"Sofort logo. Format: Base64-encoded string.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"logo\",\n    \"currencyCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-sofort-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SofortInfo
---
