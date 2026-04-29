---
description: DotpayDetails schema from Adyen API
layout: schema
name: DotpayDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The Dotpay issuer value of the shopper's selected bank. Set this to an **id** of a Dotpay issuer to preselect it.
  name: issuer
  type: string
- description: '**dotpay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-dotpay-details-schema.json
slug: checkout-dotpay-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-dotpay-details-schema.json\",\n  \"title\": \"DotpayDetails\",\n  \"description\": \"DotpayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The Dotpay issuer value of the shopper's selected bank. Set this to an **id** of a Dotpay issuer to preselect it.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"dotpay\",\n      \"description\": \"**dotpay**\",\n      \"enum\": [\n        \"dotpay\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"issuer\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-dotpay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DotpayDetails
---
