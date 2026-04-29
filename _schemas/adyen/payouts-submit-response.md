---
description: SubmitResponse schema from Adyen API
layout: schema
name: SubmitResponse
properties_list:
- description: This field contains additional data, which may be returned in a particular response.
  name: additionalData
  type: object
- description: A new reference to uniquely identify this request.
  name: pspReference
  type: string
- description: In case of refusal, an informational message for the reason.
  name: refusalReason
  type: string
- description: 'The response: * In case of success, it is `payout-submit-received`. * In case of an error, an informational message is returned.'
  name: resultCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-submit-response-schema.json
slug: payouts-submit-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-submit-response-schema.json\",\n  \"title\": \"SubmitResponse\",\n  \"description\": \"SubmitResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"additionalData\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"This field contains additional data, which may be returned in a particular response.\",\n      \"type\": \"object\"\n    },\n    \"pspReference\": {\n      \"description\": \"A new reference to uniquely identify this request.\",\n      \"type\": \"string\"\n    },\n    \"refusalReason\": {\n      \"description\": \"In case of refusal, an informational message for the reason.\",\n      \"type\": \"string\"\n    },\n    \"resultCode\": {\n      \"description\": \"The response:\\n* In case of success, it is `payout-submit-received`.\\\
  n* In case of an error, an informational message is returned.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"pspReference\",\n    \"resultCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-submit-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SubmitResponse
---
