---
description: SweepCounterparty schema from Adyen API
layout: schema
name: SweepCounterparty
properties_list:
- description: The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id). You can only use this for periodic
  name: balanceAccountId
  type: string
- description: The merchant account that will be the source of funds, if you are processing payments with Adyen. You can only use this with sweeps of `type` **pull** and `schedule.type` **balance**.
  name: merchantAccount
  type: string
- description: The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/transferInstruments__resParam_id). You can also use this in c
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/notification-webhooks-sweep-counterparty-schema.json
slug: notification-webhooks-sweep-counterparty
source_filename: notification-webhooks-sweep-counterparty-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-counterparty-schema.json\",\n  \"title\": \"SweepCounterparty\",\n  \"description\": \"SweepCounterparty schema from Adyen API\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\\n\\n You can only use this for periodic sweep schedules such as `schedule.type` **daily** or **monthly**.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that will be the source of funds, if you are processing payments with Adyen. You can only use this with sweeps of `type` **pull** and `schedule.type` **balance**.\",\n      \"type\": \"string\"\n    },\n\
  \    \"transferInstrumentId\": {\n      \"description\": \"The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/transferInstruments__resParam_id).\\n\\nYou can also use this in combination with a `merchantAccount` and a `type` **pull** to start a direct debit request from the source transfer instrument. To use this feature, reach out to your Adyen contact.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/notification-webhooks-sweep-counterparty-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepCounterparty
---
