---
description: PaymentResult schema from Adyen API
layout: schema
name: PaymentResult
properties_list:
- description: ''
  name: PaymentType
  type: object
- description: ''
  name: PaymentInstrumentData
  type: object
- description: ''
  name: AmountsResp
  type: object
- description: ''
  name: Instalment
  type: object
- description: ''
  name: CurrencyConversion
  type: array
- description: ''
  name: MerchantOverrideFlag
  type: boolean
- description: ''
  name: CapturedSignature
  type: object
- description: ''
  name: ProtectedSignature
  type: string
- description: ''
  name: CustomerLanguage
  type: string
- description: ''
  name: OnlineFlag
  type: boolean
- description: ''
  name: AuthenticationMethod
  type: object
- description: ''
  name: ValidityDate
  type: string
- description: ''
  name: PaymentAcquirerData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-result-schema.json
slug: terminal-payment-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-result-schema.json\",\n  \"title\": \"PaymentResult\",\n  \"description\": \"PaymentResult schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentType\": {\n      \"$ref\": \"#/components/schemas/PaymentType\"\n    },\n    \"PaymentInstrumentData\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentData\"\n    },\n    \"AmountsResp\": {\n      \"$ref\": \"#/components/schemas/AmountsResp\"\n    },\n    \"Instalment\": {\n      \"$ref\": \"#/components/schemas/Instalment\"\n    },\n    \"CurrencyConversion\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CurrencyConversion\"\n      }\n    },\n    \"MerchantOverrideFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"CapturedSignature\"\
  : {\n      \"$ref\": \"#/components/schemas/CapturedSignature\"\n    },\n    \"ProtectedSignature\": {\n      \"type\": \"string\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\"\n    },\n    \"OnlineFlag\": {\n      \"type\": \"boolean\",\n      \"default\": true\n    },\n    \"AuthenticationMethod\": {\n      \"$ref\": \"#/components/schemas/AuthenticationMethod\"\n    },\n    \"ValidityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"PaymentAcquirerData\": {\n      \"$ref\": \"#/components/schemas/PaymentAcquirerData\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-result-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentResult
---
