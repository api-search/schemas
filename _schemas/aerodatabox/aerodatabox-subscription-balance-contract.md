---
description: Represents the balance for all alert subscriptions associated with the user acount, including remaining credits and timestamps for the most recent refill and deduction operations.
layout: schema
name: SubscriptionBalanceContract
properties_list:
- description: Alert credits remaining for the account.
  name: creditsRemaining
  type: integer
- description: The datetime when the balance was last re-filled, in UTC.
  name: lastRefilledUtc
  type: string
- description: The datetime when the balance was last deducated, in UTC. Deduction typically occurs when an alert notification was dispatched for one of the alert subscriptions associated with the user account.
  name: lastDeductedUtc
  type: string
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-subscription-balance-contract-schema.json
slug: aerodatabox-subscription-balance-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-balance-contract-schema.json\",\n  \"title\": \"SubscriptionBalanceContract\",\n  \"description\": \"Represents the balance for all alert subscriptions associated with the user acount, including remaining credits and timestamps\\r\\nfor the most recent refill and deduction operations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"creditsRemaining\": {\n      \"type\": \"integer\",\n      \"description\": \"Alert credits remaining for the account.\",\n      \"format\": \"int64\"\n    },\n    \"lastRefilledUtc\": {\n      \"type\": \"string\",\n      \"description\": \"The datetime when the balance was last re-filled, in UTC.\",\n      \"format\": \"date-time\"\n    },\n    \"lastDeductedUtc\": {\n      \"type\": \"string\",\n      \"description\": \"The datetime when the balance\
  \ was last deducated, in UTC.\\r\\nDeduction typically occurs when an alert notification was dispatched\\r\\nfor one of the alert subscriptions associated with the user account.\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"creditsRemaining\",\n    \"lastDeductedUtc\",\n    \"lastRefilledUtc\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-subscription-balance-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: SubscriptionBalanceContract
---
