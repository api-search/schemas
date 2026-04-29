---
description: StoreDetailResponse schema from Adyen API
layout: schema
name: StoreDetailResponse
properties_list:
- description: This field contains additional data, which may be returned in a particular response.
  name: additionalData
  type: object
- description: A new reference to uniquely identify this request.
  name: pspReference
  type: string
- description: The token which you can use later on for submitting the payout.
  name: recurringDetailReference
  type: string
- description: The result code of the transaction. `Success` indicates that the details were stored successfully.
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-store-detail-response-schema.json
slug: payouts-store-detail-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-store-detail-response-schema.json\",\n  \"title\": \"StoreDetailResponse\",\n  \"description\": \"StoreDetailResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be returned in a particular response.\",\n      \"type\": \"object\"\n    },\n    \"pspReference\": {\n      \"description\": \"A new reference to uniquely identify this request.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"description\": \"The token which you can use later on for submitting the payout.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The result code of\
  \ the transaction. `Success` indicates that the details were stored successfully.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"recurringDetailReference\",\n    \"resultCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-store-detail-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: StoreDetailResponse
---
