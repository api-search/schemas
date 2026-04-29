---
description: GiroPayInfo schema from Adyen API
layout: schema
name: GiroPayInfo
properties_list:
- description: The email address of merchant support.
  name: supportEmail
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-giro-pay-info-schema.json
slug: management-giro-pay-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-giro-pay-info-schema.json\",\n  \"title\": \"GiroPayInfo\",\n  \"description\": \"GiroPayInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"supportEmail\": {\n      \"description\": \"The email address of merchant support.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"supportEmail\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-giro-pay-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: GiroPayInfo
---
