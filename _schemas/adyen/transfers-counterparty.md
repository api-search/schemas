---
description: Counterparty schema from Adyen API
layout: schema
name: Counterparty
properties_list:
- description: The identifier of the receiving account holder. The payout will default to the primary balance account of this account holder if no `balanceAccountId` is provided.
  name: accountHolderId
  type: string
- description: The identifier of the balance account that belongs to the receiving account holder.
  name: balanceAccountId
  type: string
- description: The identifier of the transfer instrument that belongs to the legal entity of the account holder.
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-counterparty-schema.json
slug: transfers-counterparty
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-counterparty-schema.json\",\n  \"title\": \"Counterparty\",\n  \"description\": \"Counterparty schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountHolderId\": {\n      \"description\": \"The identifier of the receiving account holder. The payout will default to the primary balance account of this account holder if no `balanceAccountId` is provided.\",\n      \"type\": \"string\"\n    },\n    \"balanceAccountId\": {\n      \"description\": \"The identifier of the balance account that belongs to the receiving account holder.\",\n      \"type\": \"string\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"The identifier of the transfer instrument that belongs to the legal entity of the account holder.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-counterparty-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Counterparty
---
