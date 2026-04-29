---
description: TransferNotificationCounterParty schema from Adyen API
layout: schema
name: TransferNotificationCounterParty
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
schema_file: json-schema/transfer-webhooks-transfer-notification-counter-party-schema.json
slug: transfer-webhooks-transfer-notification-counter-party
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-notification-counter-party-schema.json\",\n  \"title\": \"TransferNotificationCounterParty\",\n  \"description\": \"TransferNotificationCounterParty schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"Unique identifier of the [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"bankAccount\": {\n      \"description\": \"Contains information about the bank account.\",\n      \"$ref\": \"#/components/schemas/BankAccountV3\"\n    },\n    \"merchant\": {\n      \"description\": \"Contains information about the merchant.\",\n      \"$ref\": \"#/components/schemas/TransferNotificationMerchantData\"\n    },\n    \"\
  transferInstrumentId\": {\n      \"description\": \"Unique identifier of the [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id).\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfer-webhooks-transfer-notification-counter-party-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferNotificationCounterParty
---
