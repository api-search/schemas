---
description: CardholderReceipt schema from Adyen API
layout: schema
name: CardholderReceipt
properties_list:
- description: A custom header to show on the shopper receipt for an authorised transaction. Allows one or two comma-separated header lines, and blank lines. For example, `header,header,filler`
  name: headerForAuthorizedReceipt
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-cardholder-receipt-schema.json
slug: management-cardholder-receipt
source_filename: management-cardholder-receipt-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-cardholder-receipt-schema.json\",\n  \"title\": \"CardholderReceipt\",\n  \"description\": \"CardholderReceipt schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"headerForAuthorizedReceipt\": {\n      \"description\": \"A custom header to show on the shopper receipt for an authorised transaction. Allows one or two comma-separated header lines, and blank lines. For example, `header,header,filler`\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-cardholder-receipt-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardholderReceipt
---
