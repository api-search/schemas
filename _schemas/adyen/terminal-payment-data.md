---
description: PaymentData schema from Adyen API
layout: schema
name: PaymentData
properties_list:
- description: ''
  name: PaymentType
  type: object
- description: ''
  name: SplitPaymentFlag
  type: boolean
- description: ''
  name: RequestedValidityDate
  type: string
- description: ''
  name: CardAcquisitionReference
  type: object
- description: ''
  name: Instalment
  type: object
- description: ''
  name: CustomerOrder
  type: object
- description: ''
  name: PaymentInstrumentData
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-data-schema.json
slug: terminal-payment-data
source_filename: terminal-payment-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-data-schema.json\",\n  \"title\": \"PaymentData\",\n  \"description\": \"PaymentData schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentType\": {\n      \"$ref\": \"#/components/schemas/PaymentType\"\n    },\n    \"SplitPaymentFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    },\n    \"RequestedValidityDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"CardAcquisitionReference\": {\n      \"$ref\": \"#/components/schemas/TransactionIDType\"\n    },\n    \"Instalment\": {\n      \"$ref\": \"#/components/schemas/Instalment\"\n    },\n    \"CustomerOrder\": {\n      \"$ref\": \"#/components/schemas/CustomerOrder\"\n    },\n    \"PaymentInstrumentData\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentData\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentData
---
