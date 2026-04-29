---
description: ''
layout: schema
name: Payment
properties_list:
- description: Unique Payment Reference of the real time settlement method provided by DSP.
  name: paymentReference
  type: string
- description: Creditor or CSP requested real-time settlement method. * Refer to Codes and Formats section for more details.
  name: clearingSystem
  type: string
- description: ISO 8601 format date and time in Coordinated Universal Time (UTC), when real time settlement is initiated.
  name: paymentDateTime
  type: string
- description: The actual amount that has been transferred from the Debtor to the Creditor.
  name: paymentAmount
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-debtor-service-provider-resources-payment-schema.json
slug: mastercard-debtor-service-provider-resources-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Payment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentReference\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Payment Reference of the real time settlement method provided by DSP.\"\n    },\n    \"clearingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Creditor or CSP requested real-time settlement method. * Refer to Codes and Formats section for more details.\"\n    },\n    \"paymentDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 format date and time in Coordinated Universal Time (UTC), when real time settlement is initiated.\"\n    },\n    \"paymentAmount\": {\n      \"type\": \"string\",\n      \"description\": \"The actual amount that has been transferred from the Debtor to the Creditor.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-debtor-service-provider-resources-payment-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: Payment
---
