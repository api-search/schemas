---
description: Recurring schema from Adyen API
layout: schema
name: Recurring
properties_list:
- description: 'The type of recurring contract to be used. Possible values: * `ONECLICK` – Payment details can be used to initiate a one-click payment, where the shopper enters the [card security code (CVC/CVV)](http'
  name: contract
  type: string
- description: A descriptive name for this detail.
  name: recurringDetailName
  type: string
- description: Date after which no further authorisations shall be performed. Only for 3D Secure 2.
  name: recurringExpiry
  type: string
- description: Minimum number of days between authorisations. Only for 3D Secure 2.
  name: recurringFrequency
  type: string
- description: The name of the token service.
  name: tokenService
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payouts-recurring-schema.json
slug: payouts-recurring
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-recurring-schema.json\",\n  \"title\": \"Recurring\",\n  \"description\": \"Recurring schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contract\": {\n      \"description\": \"The type of recurring contract to be used.\\nPossible values:\\n* `ONECLICK` \\u2013 Payment details can be used to initiate a one-click payment, where the shopper enters the [card security code (CVC/CVV)](https://docs.adyen.com/payments-fundamentals/payment-glossary#card-security-code-cvc-cvv-cid).\\n* `RECURRING` \\u2013 Payment details can be used without the card security code to initiate [card-not-present transactions](https://docs.adyen.com/payments-fundamentals/payment-glossary#card-not-present-cnp).\\n* `ONECLICK,RECURRING` \\u2013 Payment details can be used regardless of whether the shopper is\
  \ on your site or not.\\n* `PAYOUT` \\u2013 Payment details can be used to [make a payout](https://docs.adyen.com/online-payments/online-payouts).\",\n      \"enum\": [\n        \"ONECLICK\",\n        \"RECURRING\",\n        \"PAYOUT\"\n      ],\n      \"type\": \"string\"\n    },\n    \"recurringDetailName\": {\n      \"description\": \"A descriptive name for this detail.\",\n      \"type\": \"string\"\n    },\n    \"recurringExpiry\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Date after which no further authorisations shall be performed. Only for 3D Secure 2.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"recurringFrequency\": {\n      \"x-addedInVersion\": \"40\",\n      \"description\": \"Minimum number of days between authorisations. Only for 3D Secure 2.\",\n      \"type\": \"string\"\n    },\n    \"tokenService\": {\n      \"x-addedInVersion\": \"25\",\n      \"description\": \"The name of the token service.\",\n      \"enum\"\
  : [\n        \"VISATOKENSERVICE\",\n        \"MCTOKENSERVICE\",\n        \"AMEXTOKENSERVICE\",\n        \"TOKEN_SHARING\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payouts-recurring-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Recurring
---
