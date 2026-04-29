---
description: TransferFundsResponse schema from Adyen API
layout: schema
name: TransferFundsResponse
properties_list:
- description: Contains field validation errors that would prevent requests from being processed.
  name: invalidFields
  type: array
- description: The value supplied by the executing user when initiating the transfer; may be used to link multiple transactions.
  name: merchantReference
  type: string
- description: The reference of a request. Can be used to uniquely identify the request.
  name: pspReference
  type: string
- description: The result code.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-transfer-funds-response-schema.json
slug: funds-transfer-funds-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transfer-funds-response-schema.json\",\n  \"title\": \"TransferFundsResponse\",\n  \"description\": \"TransferFundsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invalidFields\": {\n      \"x-addedInVersion\": \"5\",\n      \"description\": \"Contains field validation errors that would prevent requests from being processed.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ErrorFieldType\"\n      },\n      \"type\": \"array\"\n    },\n    \"merchantReference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The value supplied by the executing user when initiating the transfer; may be used to link multiple transactions.\",\n      \"type\": \"string\"\n    },\n    \"pspReference\": {\n      \"description\": \"The reference of a request.\
  \ Can be used to uniquely identify the request.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-transfer-funds-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferFundsResponse
---
