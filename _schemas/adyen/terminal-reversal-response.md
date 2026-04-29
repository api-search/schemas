---
description: It conveys Information related to the reversal processed by the POI System. Content of the Reversal Response message.
layout: schema
name: ReversalResponse
properties_list:
- description: ''
  name: Response
  type: object
- description: ''
  name: POIData
  type: object
- description: ''
  name: OriginalPOITransaction
  type: object
- description: Copy.
  name: ReversedAmount
  type: number
- description: ''
  name: CustomerOrder
  type: array
- description: ''
  name: PaymentReceipt
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-reversal-response-schema.json
slug: terminal-reversal-response
source_filename: terminal-reversal-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-response-schema.json\",\n  \"title\": \"ReversalResponse\",\n  \"description\": \"It conveys Information related to the reversal processed by the POI System. Content of the Reversal Response message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Response\": {\n      \"$ref\": \"#/components/schemas/Response\"\n    },\n    \"POIData\": {\n      \"$ref\": \"#/components/schemas/POIData\"\n    },\n    \"OriginalPOITransaction\": {\n      \"$ref\": \"#/components/schemas/OriginalPOITransaction\"\n    },\n    \"ReversedAmount\": {\n      \"type\": \"number\",\n      \"maximum\": 99999999.999999,\n      \"minimum\": 0,\n      \"description\": \"Copy.\"\n    },\n    \"CustomerOrder\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CustomerOrder\"\n\
  \      }\n    },\n    \"PaymentReceipt\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PaymentReceipt\"\n      }\n    }\n  },\n  \"required\": [\n    \"Response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-reversal-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReversalResponse
---
