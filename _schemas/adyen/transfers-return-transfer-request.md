---
description: ReturnTransferRequest schema from Adyen API
layout: schema
name: ReturnTransferRequest
properties_list:
- description: Contains information about the amount to be returned.
  name: amount
  type: object
- description: Your internal reference for the return. If you don't provide this in the request, Adyen generates a unique reference. This reference is used in all communication with you about the instruction status.
  name: reference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-return-transfer-request-schema.json
slug: transfers-return-transfer-request
source_filename: transfers-return-transfer-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-return-transfer-request-schema.json\",\n  \"title\": \"ReturnTransferRequest\",\n  \"description\": \"ReturnTransferRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"Contains information about the amount to be returned.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"reference\": {\n      \"description\": \"Your internal reference for the return. If you don't provide this in the request, Adyen generates a unique reference. This reference is used in all communication with you about the instruction status.\\n\\nWe recommend using a unique value per instruction.\\nIf you need to provide multiple references for a transaction, separate them with hyphens (\\\"-\\\").\\n\",\n      \"maxLength\": 80,\n      \"type\": \"\
  string\"\n    }\n  },\n  \"required\": [\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-return-transfer-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ReturnTransferRequest
---
