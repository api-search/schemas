---
description: If the payment receipts are printed by the Sale system and the POI or the Sale does not implement the Print exchange (Basic profile). Customer or Merchant payment receipt.
layout: schema
name: PaymentReceipt
properties_list:
- description: ''
  name: DocumentQualifier
  type: object
- description: Type of the print integrated to other prints.
  name: IntegratedPrintFlag
  type: boolean
- description: Indicate that the cardholder payment receipt requires a physical signature by the Customer.
  name: RequiredSignatureFlag
  type: boolean
- description: ''
  name: OutputContent
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-payment-receipt-schema.json
slug: terminal-payment-receipt
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-receipt-schema.json\",\n  \"title\": \"PaymentReceipt\",\n  \"description\": \"If the payment receipts are printed by the Sale system and the POI or the Sale does not implement the Print exchange (Basic profile). Customer or Merchant payment receipt.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DocumentQualifier\": {\n      \"$ref\": \"#/components/schemas/DocumentQualifier\"\n    },\n    \"IntegratedPrintFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"Type of the print integrated to other prints.\"\n    },\n    \"RequiredSignatureFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Indicate that the cardholder payment receipt requires a physical signature by the Customer.\"\n    },\n    \"OutputContent\": {\n      \"$ref\": \"\
  #/components/schemas/OutputContent\"\n    }\n  },\n  \"required\": [\n    \"DocumentQualifier\",\n    \"OutputContent\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-payment-receipt-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PaymentReceipt
---
