---
description: PurchaseInfo schema from Adyen API
layout: schema
name: PurchaseInfo
properties_list:
- description: Date of the purchase.
  name: date
  type: string
- description: Name of the merchant.
  name: merchantName
  type: string
- description: Amount of the purchase.
  name: originalAmount
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/authentication-webhooks-purchase-info-schema.json
slug: authentication-webhooks-purchase-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-purchase-info-schema.json\",\n  \"title\": \"PurchaseInfo\",\n  \"description\": \"PurchaseInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"description\": \"Date of the purchase.\",\n      \"type\": \"string\"\n    },\n    \"merchantName\": {\n      \"description\": \"Name of the merchant.\",\n      \"type\": \"string\"\n    },\n    \"originalAmount\": {\n      \"description\": \"Amount of the purchase.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    }\n  },\n  \"required\": [\n    \"merchantName\",\n    \"date\",\n    \"originalAmount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/authentication-webhooks-purchase-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PurchaseInfo
---
