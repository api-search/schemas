---
description: TapToPay schema from Adyen API
layout: schema
name: TapToPay
properties_list:
- description: The text shown on the screen during the Tap to Pay transaction.
  name: merchantDisplayName
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-tap-to-pay-schema.json
slug: management-tap-to-pay
source_filename: management-tap-to-pay-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-tap-to-pay-schema.json\",\n  \"title\": \"TapToPay\",\n  \"description\": \"TapToPay schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantDisplayName\": {\n      \"description\": \"The text shown on the screen during the Tap to Pay transaction.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-tap-to-pay-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TapToPay
---
