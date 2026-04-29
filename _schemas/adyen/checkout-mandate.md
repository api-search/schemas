---
description: Mandate schema from Adyen API
layout: schema
name: Mandate
properties_list:
- description: The billing amount (in minor units) of the recurring transactions.
  name: amount
  type: string
- description: 'The limitation rule of the billing amount. Possible values: * **max**: The transaction amount can not exceed the `amount`. * **exact**: The transaction amount should be the same as the `amount`.'
  name: amountRule
  type: string
- description: 'The rule to specify the period, within which the recurring debit can happen, relative to the mandate recurring date. Possible values: * **on**: On a specific date. * **before**: Before and on a specif'
  name: billingAttemptsRule
  type: string
- description: 'The number of the day, on which the recurring debit can happen. Should be within the same calendar month as the mandate recurring date. Possible values: 1-31 based on the `frequency`.'
  name: billingDay
  type: string
- description: End date of the billing plan, in YYYY-MM-DD format.
  name: endsAt
  type: string
- description: 'The frequency with which a shopper should be charged. Possible values: **daily**, **weekly**, **biWeekly**, **monthly**, **quarterly**, **halfYearly**, **yearly**.'
  name: frequency
  type: string
- description: The message shown by UPI to the shopper on the approval screen.
  name: remarks
  type: string
- description: Start date of the billing plan, in YYYY-MM-DD format. By default, the transaction date.
  name: startsAt
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-mandate-schema.json
slug: checkout-mandate
source_filename: checkout-mandate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mandate-schema.json\",\n  \"title\": \"Mandate\",\n  \"description\": \"Mandate schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"description\": \"The billing amount (in minor units) of the recurring transactions.\",\n      \"type\": \"string\"\n    },\n    \"amountRule\": {\n      \"description\": \"The limitation rule of the billing amount.\\n\\nPossible values:\\n * **max**: The transaction amount can not exceed the `amount`.\\n\\n * **exact**: The transaction amount should be the same as the `amount`.\\n\\n\",\n      \"enum\": [\n        \"max\",\n        \"exact\"\n      ],\n      \"type\": \"string\"\n    },\n    \"billingAttemptsRule\": {\n      \"description\": \"The rule to specify the period, within which the recurring debit can happen, relative\
  \ to the mandate recurring date.\\n\\nPossible values:\\n\\n * **on**: On a specific date.\\n\\n * **before**:  Before and on a specific date.\\n\\n * **after**: On and after a specific date.\\n\\n\",\n      \"enum\": [\n        \"on\",\n        \"before\",\n        \"after\"\n      ],\n      \"type\": \"string\"\n    },\n    \"billingDay\": {\n      \"description\": \"The number of the day, on which the recurring debit can happen. Should be within the same calendar month as the mandate recurring date.\\n\\nPossible values: 1-31 based on the `frequency`.\",\n      \"type\": \"string\"\n    },\n    \"endsAt\": {\n      \"description\": \"End date of the billing plan, in YYYY-MM-DD format.\",\n      \"type\": \"string\"\n    },\n    \"frequency\": {\n      \"description\": \"The frequency with which a shopper should be charged.\\n\\nPossible values: **daily**, **weekly**, **biWeekly**, **monthly**, **quarterly**, **halfYearly**, **yearly**.\",\n      \"enum\": [\n        \"adhoc\",\n   \
  \     \"daily\",\n        \"weekly\",\n        \"biWeekly\",\n        \"monthly\",\n        \"quarterly\",\n        \"halfYearly\",\n        \"yearly\"\n      ],\n      \"type\": \"string\"\n    },\n    \"remarks\": {\n      \"description\": \"The message shown by UPI to the shopper on the approval screen.\",\n      \"type\": \"string\"\n    },\n    \"startsAt\": {\n      \"description\": \"Start date of the billing plan, in YYYY-MM-DD format. By default, the transaction date.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"frequency\",\n    \"amount\",\n    \"endsAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-mandate-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Mandate
---
