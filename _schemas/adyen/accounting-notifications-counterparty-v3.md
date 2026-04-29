---
description: CounterpartyV3 schema from Adyen API
layout: schema
name: CounterpartyV3
properties_list:
- description: Unique identifier of the [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).
  name: balanceAccountId
  type: string
- description: Contains information about the bank account.
  name: bankAccount
  type: object
- description: Contains information about the merchant.
  name: merchant
  type: object
- description: Unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/accounting-notifications-counterparty-v3-schema.json
slug: accounting-notifications-counterparty-v3
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-counterparty-v3-schema.json\",\n  \"title\": \"CounterpartyV3\",\n  \"description\": \"CounterpartyV3 schema from Adyen API\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"Unique identifier of the [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"bankAccount\": {\n      \"description\": \"Contains information about the bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccountV3\"\n    },\n    \"merchant\": {\n      \"description\": \"Contains information about the merchant.\",\n      \"$ref\": \"#/components/schemas/MerchantData\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"Unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/accounting-notifications-counterparty-v3-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CounterpartyV3
---
