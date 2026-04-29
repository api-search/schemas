---
description: PlatformChargebackLogic schema from Adyen API
layout: schema
name: PlatformChargebackLogic
properties_list:
- description: 'The method of handling the chargeback. Possible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**, **deductAccordingToSplitRatio**.'
  name: behavior
  type: string
- description: The unique identifier of the balance account to which the chargeback fees are booked. By default, the chargeback fees are booked to your liable balance account.
  name: costAllocationAccount
  type: string
- description: The unique identifier of the balance account against which the disputed amount is booked. Required if `behavior` is **deductFromOneBalanceAccount**.
  name: targetAccount
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-platform-chargeback-logic-schema.json
slug: payments-platform-chargeback-logic
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-platform-chargeback-logic-schema.json\",\n  \"title\": \"PlatformChargebackLogic\",\n  \"description\": \"PlatformChargebackLogic schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"behavior\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The method of handling the chargeback.\\n\\nPossible values: **deductFromLiableAccount**, **deductFromOneBalanceAccount**, **deductAccordingToSplitRatio**.\",\n      \"enum\": [\n        \"deductAccordingToSplitRatio\",\n        \"deductFromLiableAccount\",\n        \"deductFromOneBalanceAccount\"\n      ],\n      \"type\": \"string\"\n    },\n    \"costAllocationAccount\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The unique identifier of the balance account to which the chargeback fees are booked. By\
  \ default, the chargeback fees are booked to your liable balance account.\",\n      \"type\": \"string\"\n    },\n    \"targetAccount\": {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The unique identifier of the balance account against which the disputed amount is booked.\\n\\nRequired if `behavior` is **deductFromOneBalanceAccount**.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-platform-chargeback-logic-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: PlatformChargebackLogic
---
