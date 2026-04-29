---
description: RefundFundsTransferRequest schema from Adyen API
layout: schema
name: RefundFundsTransferRequest
properties_list:
- description: The amount to be transferred.
  name: amount
  type: object
- description: A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.
  name: merchantReference
  type: string
- description: A PSP reference of the original fund transfer.
  name: originalReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/funds-refund-funds-transfer-request-schema.json
slug: funds-refund-funds-transfer-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-funds-transfer-request-schema.json\",\n  \"title\": \"RefundFundsTransferRequest\",\n  \"description\": \"RefundFundsTransferRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The amount to be transferred.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"merchantReference\": {\n      \"description\": \"A value that can be supplied at the discretion of the executing user in order to link multiple transactions to one another.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"A PSP reference of the original fund transfer.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"originalReference\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/funds-refund-funds-transfer-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: RefundFundsTransferRequest
---
