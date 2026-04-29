---
description: It conveys Information requested for status of the last or current Payment, Loyalty or Reversal transaction. Content of the TransactionStatus Request message.
layout: schema
name: TransactionStatusRequest
properties_list:
- description: ''
  name: MessageReference
  type: object
- description: Request to reprint the POI receipt(s).
  name: ReceiptReprintFlag
  type: boolean
- description: ''
  name: DocumentQualifier
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/terminal-transaction-status-request-schema.json
slug: terminal-transaction-status-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-status-request-schema.json\",\n  \"title\": \"TransactionStatusRequest\",\n  \"description\": \"It conveys Information requested for status of the last or current Payment, Loyalty or Reversal transaction. Content of the TransactionStatus Request message.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MessageReference\": {\n      \"$ref\": \"#/components/schemas/MessageReference\"\n    },\n    \"ReceiptReprintFlag\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Request to reprint the POI receipt(s).\"\n    },\n    \"DocumentQualifier\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DocumentQualifier\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/terminal-transaction-status-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionStatusRequest
---
