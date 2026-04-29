---
description: RefundFundsTransferResponse schema from Adyen API
layout: schema
name: RefundFundsTransferResponse
properties_list:
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The value supplied by the executing user when initiating the transfer refund; may be used to link multiple transactions.
  name: merchantReference
  type: string
- description: The message of the response.
  name: message
  type: string
- description: A PSP reference of the original fund transfer.
  name: originalReference
  type: string
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-refund-funds-transfer-response-schema.json
slug: funds-refund-funds-transfer-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-funds-transfer-response-schema.json\",\n  \"title\": \"RefundFundsTransferResponse\",\n  \"description\": \"RefundFundsTransferResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"description\": \"The value supplied by the executing user when initiating the transfer refund; may be used to link multiple transactions.\",\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"description\": \"The message of the response.\",\n      \"type\"\
  : \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"A PSP reference of the original fund transfer.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request. Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-funds-transfer-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RefundFundsTransferResponse
---
