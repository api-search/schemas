---
description: SweepCounterparty schema from Adyen API
layout: schema
name: SweepCounterparty
properties_list:
- description: The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id). You can only use this for periodic
  name: balanceAccountId
  type: string
- description: The merchant account that will be the source of funds. You can only use this parameter with sweeps of `type` **pull** and `schedule.type` **balance**, and if you are processing payments with Adyen.
  name: merchantAccount
  type: string
- description: The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/legalentity/latest/post/transferInstruments#responses-200-id) depending on the sweep `type`
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-sweep-counterparty-schema.json
slug: configuration-sweep-counterparty
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sweep-counterparty-schema.json\",\n  \"title\": \"SweepCounterparty\",\n  \"description\": \"SweepCounterparty schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the destination or source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\\n\\n You can only use this for periodic sweep schedules such as `schedule.type` **daily** or **monthly**.\",\n      \"type\": \"string\"\n    },\n    \"merchantAccount\": {\n      \"description\": \"The merchant account that will be the source of funds.\\n\\nYou can only use this parameter with sweeps of `type` **pull** and `schedule.type` **balance**, and if you are processing payments with Adyen.\",\n\
  \      \"type\": \"string\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"The unique identifier of the destination or source [transfer instrument](https://docs.adyen.com/api-explorer/legalentity/latest/post/transferInstruments#responses-200-id) depending on the sweep `type`\\n\\n. To [set up automated top-up sweeps to balance accounts](https://docs.adyen.com/marketplaces-and-platforms/top-up-balance-account/#before-you-begin), use this parameter in combination with a `merchantAccount` and a sweep `type` of **pull**. Top-up sweeps start a direct debit request from the source transfer instrument. Contact Adyen Support to enable this feature.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-sweep-counterparty-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: SweepCounterparty
---
