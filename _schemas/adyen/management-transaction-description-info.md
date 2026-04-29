---
description: TransactionDescriptionInfo schema from Adyen API
layout: schema
name: TransactionDescriptionInfo
properties_list:
- description: 'The text to be shown on the shopper''s bank statement. We recommend sending a maximum of 22 characters, otherwise banks might truncate the string. Allowed characters: **a-z**, **A-Z**, **0-9**, spaces,'
  name: doingBusinessAsName
  type: string
- description: 'The type of transaction description you want to use: - **fixed**: The transaction description set in this request is used for all payments with this payment method. - **append**: The transaction descr'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-transaction-description-info-schema.json
slug: management-transaction-description-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-transaction-description-info-schema.json\",\n  \"title\": \"TransactionDescriptionInfo\",\n  \"description\": \"TransactionDescriptionInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"doingBusinessAsName\": {\n      \"description\": \"The text to be shown on the shopper's bank statement.\\n We recommend sending a maximum of 22 characters, otherwise banks might truncate the string.\\n Allowed characters: **a-z**, **A-Z**, **0-9**, spaces, and special characters **. , ' _ - ? + * /**.\",\n      \"maxLength\": 22,\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"dynamic\",\n      \"description\": \"The type of transaction description you want to use:\\n- **fixed**: The transaction description set in this request is used for all payments with this\
  \ payment method.\\n- **append**: The transaction description set in this request is used as a base for all payments with this payment method. The [transaction description set in the request to process the payment](https://docs.adyen.com/api-explorer/Checkout/70/post/sessions#request-shopperStatement) is appended to this base description. Note that if the combined length exceeds 22 characters, banks may truncate the string.\\n- **dynamic**: Only the [transaction description set in the request to process the payment](https://docs.adyen.com/api-explorer/Checkout/70/post/sessions#request-shopperStatement) is used for payments with this payment method.\",\n      \"enum\": [\n        \"append\",\n        \"dynamic\",\n        \"fixed\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-transaction-description-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TransactionDescriptionInfo
---
