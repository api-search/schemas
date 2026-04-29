---
description: It conveys Information related to the account for which a Balance Inquiry is requested. Content of the Balance Inquiry Request message.
layout: schema
name: BalanceInquiryRequest
properties_list:
- description: ''
  name: PaymentAccountReq
  type: object
- description: ''
  name: LoyaltyAccountReq
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-balance-inquiry-request-schema.json
slug: terminal-balance-inquiry-request
source_filename: terminal-balance-inquiry-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-balance-inquiry-request-schema.json\",\n  \"title\": \"BalanceInquiryRequest\",\n  \"description\": \"It conveys Information related to the account for which a Balance Inquiry is requested. Content of the Balance Inquiry Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentAccountReq\": {\n      \"$ref\": \"#/components/schemas/PaymentAccountReq\"\n    },\n    \"LoyaltyAccountReq\": {\n      \"$ref\": \"#/components/schemas/LoyaltyAccountReq\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-balance-inquiry-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: BalanceInquiryRequest
---
