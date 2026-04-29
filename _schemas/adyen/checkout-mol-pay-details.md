---
description: MolPayDetails schema from Adyen API
layout: schema
name: MolPayDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The shopper's bank. Specify this with the issuer value that corresponds to this bank.
  name: issuer
  type: string
- description: '**molpay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-mol-pay-details-schema.json
slug: checkout-mol-pay-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mol-pay-details-schema.json\",\n  \"title\": \"MolPayDetails\",\n  \"description\": \"MolPayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The shopper's bank. Specify this with the issuer value that corresponds to this bank.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**molpay**\",\n      \"enum\": [\n        \"molpay_ebanking_fpx_MY\",\n        \"molpay_ebanking_TH\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"issuer\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mol-pay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: MolPayDetails
---
