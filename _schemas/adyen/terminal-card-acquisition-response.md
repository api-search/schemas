---
description: It conveys Information related to the payment and loyalty cards read and processed by the POI System and entered by the Customer. Content of the Card Acquisition Response message.
layout: schema
name: CardAcquisitionResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: SaleData
  type: object
- description: ''
  name: POIData
  type: object
- description: Data related to the POI System.
  name: CustomerLanguage
  type: string
- description: ''
  name: PaymentBrand
  type: array
- description: ''
  name: PaymentInstrumentData
  type: object
- description: ''
  name: LoyaltyAccount
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-card-acquisition-response-schema.json
slug: terminal-card-acquisition-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-response-schema.json\",\n  \"title\": \"CardAcquisitionResponse\",\n  \"description\": \"It conveys Information related to the payment and loyalty cards read and processed by the POI System and entered by the Customer. Content of the Card Acquisition Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"SaleData\": {\n      \"$ref\": \"#/components/schemas/SaleData\"\n    },\n    \"POIData\": {\n      \"$ref\": \"#/components/schemas/POIData\"\n    },\n    \"CustomerLanguage\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[a-z]{2,2}$\",\n      \"description\": \"Data related to the POI System.\"\n    },\n    \"PaymentBrand\": {\n      \"type\": \"array\",\n      \"items\": {\n  \
  \      \"type\": \"string\",\n        \"pattern\": \"^.+$\",\n        \"description\": \"Brands available for payment by the card and not chosen by the Customer.\"\n      }\n    },\n    \"PaymentInstrumentData\": {\n      \"$ref\": \"#/components/schemas/PaymentInstrumentData\"\n    },\n    \"LoyaltyAccount\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LoyaltyAccount\"\n      }\n    }\n  },\n  \"required\": [\n    \"Response\",\n    \"SaleData\",\n    \"POIData\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-card-acquisition-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CardAcquisitionResponse
---
