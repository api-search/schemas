---
description: Standalone schema from Adyen API
layout: schema
name: Standalone
properties_list:
- description: The default currency of the standalone payment terminal as an [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code.
  name: currencyCode
  type: string
- description: Enable standalone mode.
  name: enableStandalone
  type: boolean
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-standalone-schema.json
slug: management-standalone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-standalone-schema.json\",\n  \"title\": \"Standalone\",\n  \"description\": \"Standalone schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currencyCode\": {\n      \"description\": \"The default currency of the standalone payment terminal as an [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code.\",\n      \"maxLength\": 3,\n      \"minLength\": 3,\n      \"type\": \"string\"\n    },\n    \"enableStandalone\": {\n      \"description\": \"Enable standalone mode.\",\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-standalone-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Standalone
---
