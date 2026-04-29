---
description: AcctInfo schema from Adyen API
layout: schema
name: AcctInfo
properties_list:
- description: 'Length of time that the cardholder has had the account with the 3DS Requestor. Allowed values: * **01** — No account * **02** — Created during this transaction * **03** — Less than 30 days * **04** — '
  name: chAccAgeInd
  type: string
- description: 'Date that the cardholder’s account with the 3DS Requestor was last changed, including Billing or Shipping address, new payment account, or new user(s) added. Format: **YYYYMMDD**'
  name: chAccChange
  type: string
- description: 'Length of time since the cardholder’s account information with the 3DS Requestor was last changed, including Billing or Shipping address, new payment account, or new user(s) added. Allowed values: * *'
  name: chAccChangeInd
  type: string
- description: 'Date that cardholder’s account with the 3DS Requestor had a password change or account reset. Format: **YYYYMMDD**'
  name: chAccPwChange
  type: string
- description: 'Indicates the length of time since the cardholder’s account with the 3DS Requestor had a password change or account reset. Allowed values: * **01** — No change * **02** — Changed during this transacti'
  name: chAccPwChangeInd
  type: string
- description: 'Date that the cardholder opened the account with the 3DS Requestor. Format: **YYYYMMDD**'
  name: chAccString
  type: string
- description: 'Number of purchases with this cardholder account during the previous six months. Max length: 4 characters.'
  name: nbPurchaseAccount
  type: string
- description: 'String that the payment account was enrolled in the cardholder’s account with the 3DS Requestor. Format: **YYYYMMDD**'
  name: paymentAccAge
  type: string
- description: 'Indicates the length of time that the payment account was enrolled in the cardholder’s account with the 3DS Requestor. Allowed values: * **01** — No account (guest checkout) * **02** — During this tra'
  name: paymentAccInd
  type: string
- description: 'Number of Add Card attempts in the last 24 hours. Max length: 3 characters.'
  name: provisionAttemptsDay
  type: string
- description: 'String when the shipping address used for this transaction was first used with the 3DS Requestor. Format: **YYYYMMDD**'
  name: shipAddressUsage
  type: string
- description: 'Indicates when the shipping address used for this transaction was first used with the 3DS Requestor. Allowed values: * **01** — This transaction * **02** — Less than 30 days * **03** — 30–60 days * **'
  name: shipAddressUsageInd
  type: string
- description: 'Indicates if the Cardholder Name on the account is identical to the shipping Name used for this transaction. Allowed values: * **01** — Account Name identical to shipping Name * **02** — Account Name '
  name: shipNameIndicator
  type: string
- description: 'Indicates whether the 3DS Requestor has experienced suspicious activity (including previous fraud) on the cardholder account. Allowed values: * **01** — No suspicious activity has been observed * **02'
  name: suspiciousAccActivity
  type: string
- description: 'Number of transactions (successful and abandoned) for this cardholder account with the 3DS Requestor across all payment accounts in the previous 24 hours. Max length: 3 characters.'
  name: txnActivityDay
  type: string
- description: 'Number of transactions (successful and abandoned) for this cardholder account with the 3DS Requestor across all payment accounts in the previous year. Max length: 3 characters.'
  name: txnActivityYear
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/checkout-acct-info-schema.json
slug: checkout-acct-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-acct-info-schema.json\",\n  \"title\": \"AcctInfo\",\n  \"description\": \"AcctInfo schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chAccAgeInd\": {\n      \"description\": \"Length of time that the cardholder has had the account with the 3DS Requestor. \\nAllowed values:\\n* **01** \\u2014 No account\\n* **02** \\u2014 Created during this transaction\\n* **03** \\u2014 Less than 30 days\\n* **04** \\u2014 30\\u201360 days\\n* **05** \\u2014 More than 60 days\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"chAccChange\": {\n      \"description\": \"Date that the cardholder\\u2019s account with the 3DS Requestor was\
  \ last changed, including Billing or Shipping address, new payment account, or new user(s) added. \\nFormat: **YYYYMMDD**\",\n      \"type\": \"string\"\n    },\n    \"chAccChangeInd\": {\n      \"description\": \"Length of time since the cardholder\\u2019s account information with the 3DS Requestor was last changed, including Billing or Shipping address, new payment account, or new user(s) added. \\nAllowed values:\\n* **01** \\u2014 Changed during this transaction\\n* **02** \\u2014 Less than 30 days\\n* **03** \\u2014 30\\u201360 days\\n* **04** \\u2014 More than 60 days\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"chAccPwChange\": {\n      \"description\": \"Date that cardholder\\u2019s account with the 3DS Requestor had a password change or account reset. \\nFormat: **YYYYMMDD**\",\n      \"type\": \"string\"\n    },\n    \"chAccPwChangeInd\"\
  : {\n      \"description\": \"Indicates the length of time since the cardholder\\u2019s account with the 3DS Requestor had a password change or account reset. \\nAllowed values:\\n* **01** \\u2014 No change\\n* **02** \\u2014 Changed during this transaction\\n* **03** \\u2014 Less than 30 days\\n* **04** \\u2014 30\\u201360 days\\n* **05** \\u2014 More than 60 days\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"chAccString\": {\n      \"description\": \"Date that the cardholder opened the account with the 3DS Requestor. \\nFormat: **YYYYMMDD**\",\n      \"type\": \"string\"\n    },\n    \"nbPurchaseAccount\": {\n      \"description\": \"Number of purchases with this cardholder account during the previous six months. Max length: 4 characters.\",\n      \"type\": \"string\"\n    },\n    \"paymentAccAge\": {\n      \"description\"\
  : \"String that the payment account was enrolled in the cardholder\\u2019s account with the 3DS Requestor. \\nFormat: **YYYYMMDD**\",\n      \"type\": \"string\"\n    },\n    \"paymentAccInd\": {\n      \"description\": \"Indicates the length of time that the payment account was enrolled in the cardholder\\u2019s account with the 3DS Requestor. \\nAllowed values:\\n* **01** \\u2014 No account (guest checkout)\\n* **02** \\u2014 During this transaction\\n* **03** \\u2014 Less than 30 days\\n* **04** \\u2014 30\\u201360 days\\n* **05** \\u2014 More than 60 days\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\",\n        \"05\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"provisionAttemptsDay\": {\n      \"description\": \"Number of Add Card attempts in the last 24 hours. Max length: 3 characters.\",\n      \"type\": \"string\"\n    },\n    \"shipAddressUsage\": {\n      \"description\": \"String\
  \ when the shipping address used for this transaction was first used with the 3DS Requestor. \\nFormat: **YYYYMMDD**\",\n      \"type\": \"string\"\n    },\n    \"shipAddressUsageInd\": {\n      \"description\": \"Indicates when the shipping address used for this transaction was first used with the 3DS Requestor. \\nAllowed values:\\n* **01** \\u2014 This transaction\\n* **02** \\u2014 Less than 30 days\\n* **03** \\u2014 30\\u201360 days\\n* **04** \\u2014 More than 60 days\",\n      \"enum\": [\n        \"01\",\n        \"02\",\n        \"03\",\n        \"04\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"shipNameIndicator\": {\n      \"description\": \"Indicates if the Cardholder Name on the account is identical to the shipping Name used for this transaction. \\nAllowed values:\\n* **01** \\u2014 Account Name identical to shipping Name\\n* **02** \\u2014 Account Name different to shipping Name\",\n      \"enum\": [\n        \"\
  01\",\n        \"02\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"suspiciousAccActivity\": {\n      \"description\": \"Indicates whether the 3DS Requestor has experienced suspicious activity (including previous fraud) on the cardholder account. \\nAllowed values:\\n* **01** \\u2014 No suspicious activity has been observed\\n* **02** \\u2014 Suspicious activity has been observed\",\n      \"enum\": [\n        \"01\",\n        \"02\"\n      ],\n      \"maxLength\": 2,\n      \"minLength\": 2,\n      \"type\": \"string\"\n    },\n    \"txnActivityDay\": {\n      \"description\": \"Number of transactions (successful and abandoned) for this cardholder account with the 3DS Requestor across all payment accounts in the previous 24 hours. Max length: 3 characters.\",\n      \"maxLength\": 3,\n      \"type\": \"string\"\n    },\n    \"txnActivityYear\": {\n      \"description\": \"Number of transactions (successful and abandoned) for this\
  \ cardholder account with the 3DS Requestor across all payment accounts in the previous year. Max length: 3 characters.\",\n      \"maxLength\": 3,\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/checkout-acct-info-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AcctInfo
---
