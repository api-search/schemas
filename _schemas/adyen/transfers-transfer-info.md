---
description: TransferInfo schema from Adyen API
layout: schema
name: TransferInfo
properties_list:
- description: The amount of the transfer.
  name: amount
  type: object
- description: The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).
  name: balanceAccountId
  type: string
- description: 'The type of transfer. Possible values: - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id) or a bank account'
  name: category
  type: string
- description: The recipient of the funds transfer. A bank account, a balance account, or a transfer instrument is required.
  name: counterparty
  type: object
- description: Your description for the transfer. It is used by most banks as the transfer description. We recommend sending a maximum of 140 characters, otherwise the description may be truncated. Supported charact
  name: description
  type: string
- description: The unique identifier of the source [payment instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/paymentInstruments__resParam_id).
  name: paymentInstrumentId
  type: string
- description: 'The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**. Possible values: * **regular**'
  name: priority
  type: string
- description: Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.
  name: reference
  type: string
- description: A reference that is sent to the recipient. This reference is also sent in all webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds. Supporte
  name: referenceForBeneficiary
  type: string
- description: The ultimate sender of the funds of the transfer (ultimate debtor).
  name: ultimateParty
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/transfers-transfer-info-schema.json
slug: transfers-transfer-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-info-schema.json\",\n  \"title\": \"TransferInfo\",\n  \"description\": \"TransferInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"The amount of the transfer.\",\n      \"$ref\": \"#/components/schemas/Amount\"\n    },\n    \"balanceAccountId\": {\n      \"description\": \"The unique identifier of the source [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"category\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The type of transfer.\\n\\nPossible values:\\n\\n - **bank**: Transfer to a [transfer instrument](https://docs.adyen.com/api-explorer/#/legalentity/latest/post/transferInstruments__resParam_id)\
  \ or a bank account.\\n\\n- **internal**: Transfer to another [balance account](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/balanceAccounts__resParam_id) within your platform.\\n\\n- **issuedCard**: Transfer initiated by a Adyen-issued card.\\n\\n- **platformPayment**: Fund movements related to payments that are acquired for your users.\",\n      \"enum\": [\n        \"bank\",\n        \"internal\",\n        \"issuedCard\",\n        \"platformPayment\",\n        \"card\"\n      ],\n      \"type\": \"string\"\n    },\n    \"counterparty\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The recipient of the funds transfer. A bank account, a balance account, or a transfer instrument is required.\",\n      \"$ref\": \"#/components/schemas/CounterpartyInfoV3\"\n    },\n    \"description\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"Your description for the transfer. It is used by most banks as the transfer description. We recommend\
  \ sending a maximum of 140 characters, otherwise the description may be truncated.\\n\\nSupported characters: **[a-z] [A-Z] [0-9] / - ?** **: ( ) . , ' + Space**\\n\\nSupported characters for **regular** and **fast** transfers to a US counterparty: **[a-z] [A-Z] [0-9] & $ % # @** **~ = + - _ ' \\\" ! ?**\",\n      \"maxLength\": 140,\n      \"type\": \"string\"\n    },\n    \"paymentInstrumentId\": {\n      \"description\": \"The unique identifier of the source [payment instrument](https://docs.adyen.com/api-explorer/#/balanceplatform/latest/post/paymentInstruments__resParam_id).\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The priority for the bank transfer. This sets the speed at which the transfer is sent and the fees that you have to pay. Required for transfers with `category` **bank**.\\n\\nPossible values:\\n\\n* **regular**: For normal, low-value transactions.\\n\\n* **fast**: Faster way to transfer funds\
  \ but has higher fees. Recommended for high-priority, low-value transactions.\\n\\n* **wire**: Fastest way to transfer funds but has the highest fees. Recommended for high-priority, high-value transactions.\\n\\n* **instant**: Instant way to transfer funds in [SEPA countries](https://www.ecb.europa.eu/paym/integration/retail/sepa/html/index.en.html).\\n\\n* **crossBorder**: High-value transfer to a recipient in a different country.\\n\\n* **internal**: Transfer to an Adyen-issued business bank account (by bank account number/IBAN).\",\n      \"enum\": [\n        \"crossBorder\",\n        \"fast\",\n        \"instant\",\n        \"internal\",\n        \"regular\",\n        \"wire\"\n      ],\n      \"type\": \"string\"\n    },\n    \"reference\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Your reference for the transfer, used internally within your platform. If you don't provide this in the request, Adyen generates a unique reference.\",\n      \"maxLength\": 80,\n\
  \      \"type\": \"string\"\n    },\n    \"referenceForBeneficiary\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \" A reference that is sent to the recipient. This reference is also sent in all webhooks related to the transfer, so you can use it to track statuses for both the source and recipient of funds.\\n\\n Supported characters: **a-z**, **A-Z**, **0-9**. The maximum length depends on the `category`.\\n\\n- **internal**: 80 characters\\n\\n- **bank**: 35 characters when transferring to an IBAN, 15 characters for others.\",\n      \"maxLength\": 80,\n      \"type\": \"string\"\n    },\n    \"ultimateParty\": {\n      \"x-addedInVersion\": \"3\",\n      \"description\": \"The ultimate sender of the funds of the transfer (ultimate debtor).\",\n      \"$ref\": \"#/components/schemas/UltimatePartyIdentification\"\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"amount\",\n    \"counterparty\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/transfers-transfer-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransferInfo
---
