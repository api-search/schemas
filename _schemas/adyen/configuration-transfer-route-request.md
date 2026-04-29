---
description: TransferRouteRequest schema from Adyen API
layout: schema
name: TransferRouteRequest
properties_list:
- description: The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id). Required if `counterparty` is **transferInstrumen
  name: balanceAccountId
  type: string
- description: The unique identifier assigned to the balance platform associated with the account holder.
  name: balancePlatform
  type: string
- description: 'The type of transfer. Possible values: - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account'
  name: category
  type: string
- description: The recipient of the funds transfer. A bank account or a transfer instrument.
  name: counterparty
  type: object
- description: The two-character ISO-3166-1 alpha-2 country code of the counterparty. For example, **US** or **NL**. > Either `counterparty` or `country` field must be provided in a transfer route request.
  name: country
  type: string
- description: The three-character ISO currency code of transfer. For example, **USD** or **EUR**.
  name: currency
  type: string
- description: 'The list of priorities for the bank transfer. Priorities set the speed at which the transfer is sent and the fees that you have to pay. Multiple values can be provided. Possible values: * **regular**:'
  name: priorities
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transfer-route-request-schema.json
slug: configuration-transfer-route-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-request-schema.json\",\n  \"title\": \"TransferRouteRequest\",\n  \"description\": \"TransferRouteRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\\nRequired if `counterparty` is **transferInstrumentId**.\",\n      \"type\": \"string\"\n    },\n    \"balancePlatform\": {\n      \"description\": \"The unique identifier assigned to the balance platform associated with the account holder.\",\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"description\": \" The type of transfer. Possible values:\\n\\n  - **bank**: Transfer to a [transfer\
  \ instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account.\\n\",\n      \"enum\": [\n        \"bank\"\n      ],\n      \"type\": \"string\"\n    },\n    \"counterparty\": {\n      \"description\": \"The recipient of the funds transfer. A bank account or a transfer instrument.\",\n      \"$ref\": \"#/components/schemas/Counterparty\"\n    },\n    \"country\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code of the counterparty. For example, **US** or **NL**.\\n > Either `counterparty` or `country` field must be provided in a transfer route request.\",\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"description\": \"The three-character ISO currency code of transfer. For example, **USD** or **EUR**.\",\n      \"type\": \"string\"\n    },\n    \"priorities\": {\n      \"description\": \"The list of priorities for the bank transfer. Priorities set the speed at which the transfer\
  \ is sent and the fees that you have to pay. Multiple values can be provided.\\nPossible values:\\n\\n* **regular**: For normal, low-value transactions.\\n\\n* **fast**: Faster way to transfer funds but has higher fees. Recommended for high-priority, low-value transactions.\\n\\n* **wire**: Fastest way to transfer funds but has the highest fees. Recommended for high-priority, high-value transactions.\\n\\n* **instant**: Instant way to transfer funds in [SEPA countries](https://www.ecb.europa.eu/paym/integration/retail/sepa/html/index.en.html).\\n\\n* **crossBorder**: High-value transfer to a recipient in a different country.\\n\\n* **internal**: Transfer to an Adyen-issued business bank account (by bank account number/IBAN).\",\n      \"items\": {\n        \"enum\": [\n          \"crossBorder\",\n          \"fast\",\n          \"instant\",\n          \"internal\",\n          \"regular\",\n          \"wire\"\n        ],\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n\
  \    }\n  },\n  \"required\": [\n    \"balancePlatform\",\n    \"currency\",\n    \"category\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferRouteRequest
---
