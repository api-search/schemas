---
description: PaymentAccountReq schema from Adyen API
layout: schema
name: PaymentAccountReq
properties_list:
- description: ''
  name: AccountType
  type: object
- description: ''
  name: CardAcquisitionReference
  type: object
- description: ''
  name: PaymentInstrumentData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-account-req-schema.json
slug: terminal-payment-account-req
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-account-req-schema.json\",\n  \"title\": \"PaymentAccountReq\",\n  \"description\": \"PaymentAccountReq schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountType\": {\n      \"$ref\": \"#/components/schemas/AccountType\"\n    },\n    \"CardAcquisitionReference\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"PaymentInstrumentData\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-account-req-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentAccountReq
---
