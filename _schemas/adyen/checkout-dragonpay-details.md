---
description: DragonpayDetails schema from Adyen API
layout: schema
name: DragonpayDetails
properties_list:
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: The Dragonpay issuer value of the shopper's selected bank. Set this to an **id** of a Dragonpay issuer to preselect it.
  name: issuer
  type: string
- description: The shopper’s email address.
  name: shopperEmail
  type: string
- description: '**dragonpay**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-dragonpay-details-schema.json
slug: checkout-dragonpay-details
source_filename: checkout-dragonpay-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-dragonpay-details-schema.json\",\n  \"title\": \"DragonpayDetails\",\n  \"description\": \"DragonpayDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkoutAttemptId\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"description\": \"The Dragonpay issuer value of the shopper's selected bank. Set this to an **id** of a Dragonpay issuer to preselect it.\",\n      \"type\": \"string\"\n    },\n    \"shopperEmail\": {\n      \"description\": \"The shopper\\u2019s email address.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"**dragonpay**\",\n      \"enum\": [\n        \"dragonpay_ebanking\",\n        \"dragonpay_otc_banking\"\
  ,\n        \"dragonpay_otc_non_banking\",\n        \"dragonpay_otc_philippines\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"issuer\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-dragonpay-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DragonpayDetails
---
