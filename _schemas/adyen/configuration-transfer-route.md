---
description: TransferRoute schema from Adyen API
layout: schema
name: TransferRoute
properties_list:
- description: 'The type of transfer. Possible values: - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account'
  name: category
  type: string
- description: The two-character ISO-3166-1 alpha-2 country code of the counterparty. For example, **US** or **NL**.
  name: country
  type: string
- description: The three-character ISO currency code of transfer. For example, **USD** or **EUR**.
  name: currency
  type: string
- description: 'The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Possible values: * **regular**: For normal, low-value transactions. * **fast**:'
  name: priority
  type: string
- description: A set of rules defined by clearing houses and banking partners. Your transfer request must adhere to these rules to ensure successful initiation of transfer. Based on the priority, one or more require
  name: requirements
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/configuration-transfer-route-schema.json
slug: configuration-transfer-route
source_filename: configuration-transfer-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-schema.json\",\n  \"title\": \"TransferRoute\",\n  \"description\": \"TransferRoute schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"description\": \" The type of transfer.\\n\\n Possible values:\\n\\n  - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account.\\n\",\n      \"enum\": [\n        \"bank\",\n        \"card\",\n        \"grants\",\n        \"internal\",\n        \"issuedCard\",\n        \"migration\",\n        \"platformPayment\",\n        \"topUp\",\n        \"upgrade\"\n      ],\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"description\": \"The two-character ISO-3166-1 alpha-2 country code of the\
  \ counterparty. For example, **US** or **NL**.\",\n      \"type\": \"string\"\n    },\n    \"currency\": {\n      \"description\": \"The three-character ISO currency code of transfer. For example, **USD** or **EUR**.\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"description\": \"The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Possible values:\\n\\n* **regular**: For normal, low-value transactions.\\n\\n* **fast**: Faster way to transfer funds but has higher fees. Recommended for high-priority, low-value transactions.\\n\\n* **wire**: Fastest way to transfer funds but has the highest fees. Recommended for high-priority, high-value transactions.\\n\\n* **instant**: Instant way to transfer funds in [SEPA countries](https://www.ecb.europa.eu/paym/integration/retail/sepa/html/index.en.html).\\n\\n* **crossBorder**: High-value transfer to a recipient in a different country.\\n\\n* **internal**: Transfer\
  \ to an Adyen-issued business bank account (by bank account number/IBAN).\",\n      \"enum\": [\n        \"crossBorder\",\n        \"fast\",\n        \"instant\",\n        \"internal\",\n        \"regular\",\n        \"wire\"\n      ],\n      \"type\": \"string\"\n    },\n    \"requirements\": {\n      \"description\": \"A set of rules defined by clearing houses and banking partners. Your transfer request must adhere to these rules to ensure successful initiation of transfer. Based on the priority, one or more requirements may be returned. Each requirement is defined with a `type` and `description`.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressRequirement\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/AmountMinMaxRequirement\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/BankAccountIdentificationTypeRequirement\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/PaymentInstrumentRequirement\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/configuration-transfer-route-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferRoute
---
