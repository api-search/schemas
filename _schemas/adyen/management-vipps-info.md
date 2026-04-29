---
description: VippsInfo schema from Adyen API
layout: schema
name: VippsInfo
properties_list:
- description: 'Vipps logo. Format: Base64-encoded string.'
  name: logo
  type: string
- description: Vipps subscription cancel url (required in case of [recurring payments](https://docs.adyen.com/online-payments/tokenization))
  name: subscriptionCancelUrl
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-vipps-info-schema.json
slug: management-vipps-info
source_filename: management-vipps-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-vipps-info-schema.json\",\n  \"title\": \"VippsInfo\",\n  \"description\": \"VippsInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logo\": {\n      \"description\": \"Vipps logo. Format: Base64-encoded string.\",\n      \"type\": \"string\"\n    },\n    \"subscriptionCancelUrl\": {\n      \"description\": \"Vipps subscription cancel url (required in case of [recurring payments](https://docs.adyen.com/online-payments/tokenization))\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"logo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-vipps-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: VippsInfo
---
