---
description: A Barclays bank account as returned by the Open Banking Account Information API.
layout: schema
name: Account
properties_list:
- description: Unique identifier for the account.
  name: accountId
  type: string
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: Type of the account.
  name: accountType
  type: string
- description: Sub-type of the account.
  name: accountSubType
  type: string
- description: Customer-assigned nickname for the account.
  name: nickname
  type: string
- description: ''
  name: account
  type: array
- description: ''
  name: balances
  type: array
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/account-schema.json
slug: account
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/barclays/json-schema/account-schema.json\",\n  \"title\": \"Account\",\n  \"description\": \"A Barclays bank account as returned by the Open Banking Account Information API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the account.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"description\": \"ISO 4217 currency code.\"\n    },\n    \"accountType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Personal\", \"Business\", \"Savings\", \"CreditCard\"],\n      \"description\": \"Type of the account.\"\n    },\n    \"accountSubType\": {\n      \"type\": \"string\",\n      \"enum\": [\"CurrentAccount\", \"Savings\", \"CreditCard\", \"Loan\"],\n      \"description\": \"Sub-type of the account.\"\n    },\n    \"\
  nickname\": {\n      \"type\": \"string\",\n      \"description\": \"Customer-assigned nickname for the account.\"\n    },\n    \"account\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"schemeName\": {\n            \"type\": \"string\",\n            \"enum\": [\"UK.OBIE.SortCodeAccountNumber\", \"UK.OBIE.IBAN\"]\n          },\n          \"identification\": {\n            \"type\": \"string\",\n            \"description\": \"Account number or IBAN.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Account holder name.\"\n          }\n        },\n        \"required\": [\"schemeName\", \"identification\"]\n      }\n    },\n    \"balances\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Balance\"\n      }\n    }\n  },\n  \"required\": [\"accountId\", \"currency\", \"accountType\"],\n  \"definitions\": {\n    \"Balance\":\
  \ {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"amount\": {\n              \"type\": \"string\",\n              \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n            },\n            \"currency\": {\n              \"type\": \"string\",\n              \"pattern\": \"^[A-Z]{3}$\"\n            }\n          },\n          \"required\": [\"amount\", \"currency\"]\n        },\n        \"creditDebitIndicator\": {\n          \"type\": \"string\",\n          \"enum\": [\"Credit\", \"Debit\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"ClosingAvailable\", \"ClosingBooked\", \"ForwardAvailable\", \"InterimAvailable\", \"InterimBooked\"]\n        },\n        \"dateTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      },\n      \"required\": [\"amount\", \"creditDebitIndicator\", \"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/barclays/refs/heads/main/json-schema/account-schema.json
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: Account
---
