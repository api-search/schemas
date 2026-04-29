---
description: AchNotificationOfChangeNotificationRequestDataNoc schema from Adyen API
layout: schema
name: AchNotificationOfChangeNotificationRequestDataNoc
properties_list:
- description: New bank account number.
  name: newBankAccountNumber
  type: string
- description: 'New bank account type. Possible values: * **Savings** * **Checking**'
  name: newBankAccountType
  type: string
- description: New branch code.
  name: newBranchCode
  type: string
- description: 'Notification of Change reason code. Possible values: * **C01** : Incorrect bank account number. * **C02** : Incorrect transit/routing number. * **C03** : Incorrect transit/routing number and bank acco'
  name: reasonCode
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/webhooks-ach-notification-of-change-notification-request-data-noc-schema.json
slug: webhooks-ach-notification-of-change-notification-request-data-noc
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-data-noc-schema.json\",\n  \"title\": \"AchNotificationOfChangeNotificationRequestDataNoc\",\n  \"description\": \"AchNotificationOfChangeNotificationRequestDataNoc schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"newBankAccountNumber\": {\n      \"description\": \"New bank account number.\",\n      \"type\": \"string\"\n    },\n    \"newBankAccountType\": {\n      \"description\": \"New bank account type.\\n\\nPossible values:\\n*  **Savings**\\n*  **Checking**\\n\\n\",\n      \"enum\": [\n        \"Checking\",\n        \"Savings\"\n      ],\n      \"type\": \"string\"\n    },\n    \"newBranchCode\": {\n      \"description\": \"New branch code.\",\n      \"type\": \"string\"\n    },\n    \"reasonCode\": {\n      \"description\"\
  : \"Notification of Change reason code.\\n\\nPossible values:\\n*  **C01** : Incorrect bank account number.\\n*  **C02** : Incorrect transit/routing number.\\n*  **C03** : Incorrect transit/routing number and bank account number.\\n*  **C04** : Bank account name change.\\n*  **C05** : Incorrect payment code.\\n*  **C06** : Incorrect bank account number and transit code.\\n*  **C07** : Incorrect transit/routing number, bank account number and payment code.\\n*  **C09** : Incorrect individual ID number.\\n*  **C10** : Incorrect company name.\\n*  **C11** : Incorrect company identification.\\n*  **C12** : Incorrect company name and company ID.\\n\\n\",\n      \"enum\": [\n        \"C01\",\n        \"C02\",\n        \"C03\",\n        \"C04\",\n        \"C05\",\n        \"C06\",\n        \"C07\",\n        \"C09\",\n        \"C10\",\n        \"C11\",\n        \"C12\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"reasonCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/webhooks-ach-notification-of-change-notification-request-data-noc-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AchNotificationOfChangeNotificationRequestDataNoc
---
