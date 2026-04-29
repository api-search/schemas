---
description: DokuDetails schema from Adyen API
layout: schema
name: DokuDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The shopper's first name.
  name: firstName
  type: string
- description: The shopper's last name.
  name: lastName
  type: string
- description: The shopper's email.
  name: shopperEmail
  type: string
- description: '**doku**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-doku-details-schema.json
slug: checkout-doku-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-doku-details-schema.json\",\n  \"title\": \"DokuDetails\",\n  \"description\": \"DokuDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"firstName\": {\n      \"description\": \"The shopper's first name.\",\n      \"type\": \"string\"\n    },\n    \"lastName\": {\n      \"description\": \"The shopper's last name.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper's email.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**doku**\",\n      \"enum\": [\n        \"doku_mandiri_va\",\n        \"doku_cimb_va\",\n        \"doku_danamon_va\"\
  ,\n        \"doku_bni_va\",\n        \"doku_permata_lite_atm\",\n        \"doku_bri_va\",\n        \"doku_bca_va\",\n        \"doku_alfamart\",\n        \"doku_indomaret\",\n        \"doku_wallet\",\n        \"doku_ovo\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"firstName\",\n    \"lastName\",\n    \"shopperEmail\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-doku-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DokuDetails
---
