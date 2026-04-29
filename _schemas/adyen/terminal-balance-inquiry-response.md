---
description: It conveys the balance and the identification of the associated payment, loyalty or stored value account. Content of the Balance Inquiry Response message.
layout: schema
name: BalanceInquiryResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: PaymentAccountStatus
  type: object
- description: ''
  name: LoyaltyAccountStatus
  type: object
- description: ''
  name: PaymentReceipt
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-balance-inquiry-response-schema.json
slug: terminal-balance-inquiry-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-balance-inquiry-response-schema.json\",\n  \"title\": \"BalanceInquiryResponse\",\n  \"description\": \"It conveys the balance and the identification of the associated payment, loyalty or stored value account. Content of the Balance Inquiry Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"PaymentAccountStatus\": {\n      \"$ref\": \"#/components/schemas/PaymentAccountStatus\"\n    },\n    \"LoyaltyAccountStatus\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccountStatus\"\n    },\n    \"PaymentReceipt\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentReceipt\"\n      }\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-balance-inquiry-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceInquiryResponse
---
