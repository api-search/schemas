---
description: Sent in the result of the payment transaction. For a card, it could also be sent in the CardAcquisition response, to be processed by the Sale System. Data related to the instrument of payment for the transaction.
layout: schema
name: PaymentInstrumentData
properties_list:
- description: ''
  name: PaymentInstrumentType
  type: object
- description: ''
  name: ProtectedCardData
  type: string
- description: ''
  name: CardData
  type: object
- description: ''
  name: CheckData
  type: object
- description: ''
  name: MobileData
  type: object
- description: ''
  name: StoredValueAccountID
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-instrument-data-schema.json
slug: terminal-payment-instrument-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-instrument-data-schema.json\",\n  \"title\": \"PaymentInstrumentData\",\n  \"description\": \"Sent in the result of the payment transaction. For a card, it could also be sent in the CardAcquisition response, to be processed by the Sale System. Data related to the instrument of payment for the transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentInstrumentType\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentType\"\n    },\n    \"ProtectedCardData\": {\n      \"type\": \"string\"\n    },\n    \"CardData\": {\n      \"$ref\": \"#/components/schemas/CardData\"\n    },\n    \"CheckData\": {\n      \"$ref\": \"#/components/schemas/CheckData\"\n    },\n    \"MobileData\": {\n      \"$ref\": \"#/components/schemas/MobileData\"\n    },\n    \"StoredValueAccountID\": {\n\
  \      \"$ref\": \"#/components/schemas/StoredValueAccountID\"\n    }\n  },\n  \"required\": [\n    \"PaymentInstrumentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-instrument-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentInstrumentData
---
