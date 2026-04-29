---
description: ModifyResponse schema from Adyen API
layout: schema
name: ModifyResponse
properties_list:
- description: This field contains additional data, which may be returned in a particular response.
  name: additionalData
  type: object
- description: Adyen's 16-character string reference associated with the transaction. This value is globally unique; quote it when communicating with us about this response.
  name: pspReference
  type: string
- description: 'The response: * In case of success, it is either `payout-confirm-received` or `payout-decline-received`. * In case of an error, an informational message is returned.'
  name: response
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-modify-response-schema.json
slug: payouts-modify-response
source_filename: payouts-modify-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-modify-response-schema.json\",\n  \"title\": \"ModifyResponse\",\n  \"description\": \"ModifyResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be returned in a particular response.\",\n      \"type\": \"object\"\n    },\n    \"pspReference\": {\n      \"description\": \"Adyen's 16-character string reference associated with the transaction. This value is globally unique; quote it when communicating with us about this response.\",\n      \"type\": \"string\"\n    },\n    \"response\": {\n      \"description\": \"The response:\\n* In case of success, it is either `payout-confirm-received` or `payout-decline-received`.\\\
  n* In case of an error, an informational message is returned.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"response\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-modify-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ModifyResponse
---
