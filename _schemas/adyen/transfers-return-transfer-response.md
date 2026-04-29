---
description: ReturnTransferResponse schema from Adyen API
layout: schema
name: ReturnTransferResponse
properties_list:
- description: The unique identifier of the return.
  name: id
  type: string
- description: Your internal reference for the return.
  name: reference
  type: string
- description: 'The resulting status of the return. Possible values: **Authorised**, **Declined**.'
  name: status
  type: string
- description: The unique identifier of the original transfer.
  name: transferId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-return-transfer-response-schema.json
slug: transfers-return-transfer-response
source_filename: transfers-return-transfer-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-return-transfer-response-schema.json\",\n  \"title\": \"ReturnTransferResponse\",\n  \"description\": \"ReturnTransferResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The unique identifier of the return.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your internal reference for the return.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The resulting status of the return.\\n\\nPossible values: **Authorised**, **Declined**.\",\n      \"enum\": [\n        \"Authorised\",\n        \"Declined\"\n      ],\n      \"type\": \"string\"\n    },\n    \"transferId\": {\n      \"description\": \"The unique identifier of the original transfer.\",\n      \"type\": \"string\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-return-transfer-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReturnTransferResponse
---
