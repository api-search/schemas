---
description: AchDetails schema from Adyen API
layout: schema
name: AchDetails
properties_list:
- description: The bank account number (without separators).
  name: bankAccountNumber
  type: string
- description: The bank account type (checking, savings...).
  name: bankAccountType
  type: string
- description: The bank routing number of the account. The field value is `nil` in most cases.
  name: bankLocationId
  type: string
- description: The checkout attempt identifier.
  name: checkoutAttemptId
  type: string
- description: Encrypted bank account number. The bank account number (without separators).
  name: encryptedBankAccountNumber
  type: string
- description: Encrypted location id. The bank routing number of the account. The field value is `nil` in most cases.
  name: encryptedBankLocationId
  type: string
- description: The name of the bank account holder. If you submit a name with non-Latin characters, we automatically replace some of them with corresponding Latin characters to meet the FATF recommendations. For exa
  name: ownerName
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: recurringDetailReference
  type: string
- description: This is the `recurringDetailReference` returned in the response when you created the token.
  name: storedPaymentMethodId
  type: string
- description: '**ach**'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-ach-details-schema.json
slug: checkout-ach-details
source_filename: checkout-ach-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-ach-details-schema.json\",\n  \"title\": \"AchDetails\",\n  \"description\": \"AchDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bankAccountNumber\": {\n      \"description\": \"The bank account number (without separators).\",\n      \"type\": \"string\"\n    },\n    \"bankAccountType\": {\n      \"description\": \"The bank account type (checking, savings...).\",\n      \"enum\": [\n        \"balance\",\n        \"checking\",\n        \"deposit\",\n        \"general\",\n        \"other\",\n        \"payment\",\n        \"savings\"\n      ],\n      \"type\": \"string\"\n    },\n    \"bankLocationId\": {\n      \"description\": \"The bank routing number of the account. The field value is `nil` in most cases.\",\n      \"type\": \"string\"\n    },\n    \"checkoutAttemptId\"\
  : {\n      \"x-addedInVersion\": \"68\",\n      \"description\": \"The checkout attempt identifier.\",\n      \"type\": \"string\"\n    },\n    \"encryptedBankAccountNumber\": {\n      \"description\": \"Encrypted bank account number. The bank account number (without separators).\",\n      \"type\": \"string\"\n    },\n    \"encryptedBankLocationId\": {\n      \"description\": \"Encrypted location id. The bank routing number of the account. The field value is `nil` in most cases.\",\n      \"type\": \"string\"\n    },\n    \"ownerName\": {\n      \"description\": \"The name of the bank account holder.\\nIf you submit a name with non-Latin characters, we automatically replace some of them with corresponding Latin characters to meet the FATF recommendations. For example:\\n* \\u03c712 is converted to ch12.\\n* \\u00fcA is converted to euA.\\n* Peter M\\u00f8ller is converted to Peter Mller, because banks don't accept '\\u00f8'.\\nAfter replacement, the ownerName must have at least three\
  \ alphanumeric characters (A-Z, a-z, 0-9), and at least one of them must be a valid Latin character (A-Z, a-z). For example:\\n* John17 - allowed.\\n* J17 - allowed.\\n* 171 - not allowed.\\n* John-7 - allowed.\\n> If provided details don't match the required format, the response returns the error message: 203 'Invalid bank account holder name'.\",\n      \"type\": \"string\"\n    },\n    \"recurringDetailReference\": {\n      \"deprecated\": true,\n      \"x-deprecatedInVersion\": \"49\",\n      \"x-deprecatedMessage\": \"Use `storedPaymentMethodId` instead.\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"type\": \"string\"\n    },\n    \"storedPaymentMethodId\": {\n      \"x-addedInVersion\": \"49\",\n      \"description\": \"This is the `recurringDetailReference` returned in the response when you created the token.\",\n      \"maxLength\": 64,\n      \"type\": \"string\"\n    },\n    \"type\": {\n \
  \     \"default\": \"ach\",\n      \"description\": \"**ach**\",\n      \"enum\": [\n        \"ach\",\n        \"ach_plaid\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"bankAccountNumber\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-ach-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AchDetails
---
