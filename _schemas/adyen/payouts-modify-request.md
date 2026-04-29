---
description: ModifyRequest schema from Adyen API
layout: schema
name: ModifyRequest
properties_list:
- description: This field contains additional data, which may be required for a particular payout request.
  name: additionalData
  type: object
- description: The merchant account identifier, with which you want to process the transaction.
  name: merchantAccount
  type: string
- description: The PSP reference received in the `/submitThirdParty` response.
  name: originalReference
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-modify-request-schema.json
slug: payouts-modify-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-modify-request-schema.json\",\n  \"title\": \"ModifyRequest\",\n  \"description\": \"ModifyRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be required for a particular payout request.\",\n      \"type\": \"object\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account identifier, with which you want to process the transaction.\",\n      \"type\": \"string\"\n    },\n    \"originalReference\": {\n      \"description\": \"The PSP reference received in the `/submitThirdParty` response.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"merchantAccount\",\n \
  \   \"originalReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-modify-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ModifyRequest
---
