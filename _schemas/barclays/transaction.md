---
description: A Barclays account transaction as returned by the Transactions API.
layout: schema
name: Transaction
properties_list:
- description: Account identifier the transaction belongs to.
  name: accountId
  type: string
- description: Unique transaction identifier.
  name: transactionId
  type: string
- description: Whether the transaction credits or debits the account.
  name: creditDebitIndicator
  type: string
- description: Settlement status of the transaction.
  name: status
  type: string
- description: Date and time the transaction was booked.
  name: bookingDateTime
  type: string
- description: Value date and time of the transaction.
  name: valueDateTime
  type: string
- description: ''
  name: amount
  type: object
- description: ''
  name: merchantDetails
  type: object
- description: Narrative description of the transaction.
  name: transactionInformation
  type: string
provider_name: Barclays
provider_slug: barclays
schema_file: json-schema/transaction-schema.json
slug: transaction
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/barclays/json-schema/transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"A Barclays account transaction as returned by the Transactions API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account identifier the transaction belongs to.\"\n    },\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier.\"\n    },\n    \"creditDebitIndicator\": {\n      \"type\": \"string\",\n      \"enum\": [\"Credit\", \"Debit\"],\n      \"description\": \"Whether the transaction credits or debits the account.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Booked\", \"Pending\"],\n      \"description\": \"Settlement status of the transaction.\"\n    },\n    \"bookingDateTime\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the transaction was booked.\"\n    },\n    \"valueDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Value date and time of the transaction.\"\n    },\n    \"amount\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"amount\": {\n          \"type\": \"string\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d{2}$\"\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{3}$\"\n        }\n      },\n      \"required\": [\"amount\", \"currency\"]\n    },\n    \"merchantDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"merchantName\": {\n          \"type\": \"string\"\n        },\n        \"merchantCategoryCode\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"transactionInformation\": {\n      \"type\": \"string\",\n      \"description\": \"Narrative\
  \ description of the transaction.\"\n    }\n  },\n  \"required\": [\"accountId\", \"transactionId\", \"creditDebitIndicator\", \"status\", \"amount\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/barclays/refs/heads/main/json-schema/transaction-schema.json
tags:
- Banking
- Credit Cards
- Finance
- Open Banking
- Payments
- PSD2
- UK Banking
title: Transaction
---
