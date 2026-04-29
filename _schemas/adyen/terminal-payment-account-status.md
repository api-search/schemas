---
description: PaymentAccountStatus schema from Adyen API
layout: schema
name: PaymentAccountStatus
properties_list:
- description: ''
  name: PaymentInstrumentData
  type: object
- description: ''
  name: CurrentBalance
  type: number
- description: ''
  name: Currency
  type: string
- description: ''
  name: PaymentAcquirerData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-account-status-schema.json
slug: terminal-payment-account-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-account-status-schema.json\",\n  \"title\": \"PaymentAccountStatus\",\n  \"description\": \"PaymentAccountStatus schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentInstrumentData\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentData\"\n    },\n    \"CurrentBalance\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3,3}$\"\n    },\n    \"PaymentAcquirerData\": {\n      \"$ref\": \"#/components/schemas/PaymentAcquirerData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-account-status-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentAccountStatus
---
