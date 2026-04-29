---
description: Allows acquisition of the card data by the Sale System before the Payment, CardAcquisition or BalanceInquiry request to the POI. It could also be sent in the CardAcquisition response, to be processed by the Sale System. Information related to the payment card used for the transaction.
layout: schema
name: CardData
properties_list:
- description: If card PAN is readable .
  name: PaymentBrand
  type: string
- description: ''
  name: MaskedPan
  type: string
- description: ''
  name: PaymentAccountRef
  type: string
- description: ''
  name: EntryMode
  type: object
- description: If available in the card.
  name: CardCountryCode
  type: integer
- description: SensitiveCardData protected by CMS EnvelopedData.
  name: ProtectedCardData
  type: string
- description: ''
  name: SensitiveCardData
  type: object
- description: ''
  name: AllowedProductCode
  type: array
- description: ''
  name: AllowedProduct
  type: array
- description: ''
  name: PaymentToken
  type: object
- description: ''
  name: CustomerOrder
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-data-schema.json
slug: terminal-card-data
source_filename: terminal-card-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-data-schema.json\",\n  \"title\": \"CardData\",\n  \"description\": \"Allows acquisition of the card data by the Sale System before the Payment, CardAcquisition  or BalanceInquiry request to the POI. It could also be sent in the CardAcquisition response, to be processed by the Sale System. Information related to the payment card used for the transaction.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PaymentBrand\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\",\n      \"description\": \"If card PAN is readable .\"\n    },\n    \"MaskedPan\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"PaymentAccountRef\": {\n      \"type\": \"string\",\n      \"pattern\": \"^.+$\"\n    },\n    \"EntryMode\": {\n      \"$ref\": \"#/components/schemas/EntryMode\"\
  \n    },\n    \"CardCountryCode\": {\n      \"type\": \"integer\",\n      \"minimum\": 3,\n      \"maximum\": 3,\n      \"description\": \"If available in the card.\"\n    },\n    \"ProtectedCardData\": {\n      \"type\": \"string\",\n      \"description\": \"SensitiveCardData protected by CMS EnvelopedData.\"\n    },\n    \"SensitiveCardData\": {\n      \"$ref\": \"#/components/schemas/SensitiveCardData\"\n    },\n    \"AllowedProductCode\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"minimum\": 1,\n        \"maximum\": 20\n      }\n    },\n    \"AllowedProduct\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AllowedProduct\"\n      }\n    },\n    \"PaymentToken\": {\n      \"$ref\": \"#/components/schemas/PaymentToken\"\n    },\n    \"CustomerOrder\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CustomerOrder\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-data-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardData
---
