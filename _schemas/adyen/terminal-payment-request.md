---
description: Request sent to terminal to initiate payment. It conveys Information related to the Payment transaction to process. Content of the Payment Request message.
layout: schema
name: PaymentRequest
properties_list:
- description: ''
  name: SaleData
  type: object
- description: ''
  name: PaymentTransaction
  type: object
- description: ''
  name: PaymentData
  type: object
- description: ''
  name: LoyaltyData
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-request-schema.json
slug: terminal-payment-request
source_filename: terminal-payment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-request-schema.json\",\n  \"title\": \"PaymentRequest\",\n  \"description\": \"Request sent to terminal to initiate payment.  It conveys Information related to the Payment transaction to process. Content of the Payment Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"PaymentTransaction\": {\n      \"$ref\": \"#/components/schemas/PaymentTransaction\"\n    },\n    \"PaymentData\": {\n      \"$ref\": \"#/components/schemas/PaymentData\"\n    },\n    \"LoyaltyData\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoyaltyData\"\n      }\n    }\n  },\n  \"required\": [\n    \"SaleData\",\n    \"PaymentTransaction\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentRequest
---
