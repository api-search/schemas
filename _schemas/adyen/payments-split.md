---
description: Split schema from Adyen API
layout: schema
name: Split
properties_list:
- description: The unique identifier of the account to which the split amount is booked. Required if `type` is **MarketPlace** or **BalanceAccount**. * [Classic Platforms integration](https://docs.adyen.com/marketpl
  name: account
  type: string
- description: The amount of the split item. * Required for all split types in the [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic). * Required if `type` is **BalanceAccount
  name: amount
  type: object
- description: Your description for the split item.
  name: description
  type: string
- description: Your unique reference for the split item. This is required if `type` is **MarketPlace** ([Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic)) or **BalanceAccount
  name: reference
  type: string
- description: 'The type of the split item. Possible values: * [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic): **Commission**, **Default**, **Marketplace**, **PaymentFee**,'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/payments-split-schema.json
slug: payments-split
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-split-schema.json\",\n  \"title\": \"Split\",\n  \"description\": \"Split schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"account\": {\n      \"description\": \"The unique identifier of the account to which the split amount is booked. Required if `type` is **MarketPlace** or **BalanceAccount**.\\n\\n* [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic): The [`accountCode`](https://docs.adyen.com/api-explorer/Account/latest/post/updateAccount#request-accountCode) of the account to which the split amount is booked.\\n* [Balance Platform](https://docs.adyen.com/marketplaces-and-platforms): The [`balanceAccountId`](https://docs.adyen.com/api-explorer/balanceplatform/latest/get/balanceAccounts/_id_#path-id) of the account to which the split\
  \ amount is booked.\",\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"description\": \"The amount of the split item.\\n\\n* Required for all split types in the [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic).\\n* Required if `type` is **BalanceAccount**, **Commission**, **Default**, or **VAT** in your [Balance Platform](https://docs.adyen.com/marketplaces-and-platforms) integration.\",\n      \"$ref\": \"#/components/schemas/SplitAmount\"\n    },\n    \"description\": {\n      \"description\": \"Your description for the split item.\",\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"description\": \"Your unique reference for the split item.\\n\\nThis is required if `type` is **MarketPlace** ([Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic)) or **BalanceAccount** ([Balance Platform](https://docs.adyen.com/marketplaces-and-platforms)).\\n\\nFor the other types, we also\
  \ recommend providing a **unique** reference so you can reconcile the split and the associated payment in the transaction overview and in the reports.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"The type of the split item.\\n\\nPossible values:\\n\\n* [Classic Platforms integration](https://docs.adyen.com/marketplaces-and-platforms/classic): **Commission**, **Default**, **Marketplace**, **PaymentFee**, **VAT**.\\n* [Balance Platform](https://docs.adyen.com/marketplaces-and-platforms): **BalanceAccount**, **Commission**, **Default**, **PaymentFee**, **Remainder**, **Surcharge**, **Tip**, **VAT**.\",\n      \"enum\": [\n        \"BalanceAccount\",\n        \"Commission\",\n        \"Default\",\n        \"MarketPlace\",\n        \"PaymentFee\",\n        \"Remainder\",\n        \"Surcharge\",\n        \"Tip\",\n        \"VAT\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/payments-split-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Split
---
