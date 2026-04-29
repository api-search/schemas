---
description: Counterparty schema from Adyen API
layout: schema
name: Counterparty
properties_list:
- description: Contains information about the bank account.
  name: bankAccount
  type: object
- description: Unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).
  name: transferInstrumentId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-counterparty-schema.json
slug: configuration-counterparty
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-counterparty-schema.json\",\n  \"title\": \"Counterparty\",\n  \"description\": \"Counterparty schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccount\": {\n      \"description\": \"Contains information about the bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccount\"\n    },\n    \"transferInstrumentId\": {\n      \"description\": \"Unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-counterparty-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Counterparty
---
