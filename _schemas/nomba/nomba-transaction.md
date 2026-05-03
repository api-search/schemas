---
description: Schema representing a Nomba transaction record for payments, transfers, and payouts across the platform.
layout: schema
name: Nomba Transaction
properties_list:
- description: The unique identifier for the transaction.
  name: transactionId
  type: string
- description: The system-generated transaction reference number.
  name: transactionRef
  type: string
- description: The merchant-provided transaction reference for idempotency and reconciliation.
  name: merchantTxRef
  type: string
- description: The transaction amount.
  name: amount
  type: number
- description: The fee charged for the transaction.
  name: fee
  type: number
- description: The ISO 4217 currency code for the transaction.
  name: currency
  type: string
- description: The transaction type indicating the direction of funds.
  name: type
  type: string
- description: The channel through which the transaction was initiated.
  name: source
  type: string
- description: The current processing status of the transaction.
  name: status
  type: string
- description: The POS terminal identifier, present for terminal-based transactions.
  name: terminalId
  type: string
- description: The Retrieval Reference Number for POS transactions.
  name: rrn
  type: string
- description: The session identifier linking related transaction steps.
  name: sessionId
  type: string
- description: A description or note associated with the transaction.
  name: narration
  type: string
- description: The date and time the transaction was created.
  name: createdAt
  type: string
- description: The date and time the transaction was last updated.
  name: updatedAt
  type: string
provider_name: Nomba
provider_slug: nomba
schema_file: json-schema/nomba-transaction-schema.json
slug: nomba-transaction
source_filename: nomba-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.nomba.com/schemas/nomba/transaction.json\",\n  \"title\": \"Nomba Transaction\",\n  \"description\": \"Schema representing a Nomba transaction record for payments, transfers, and payouts across the platform.\",\n  \"type\": \"object\",\n  \"required\": [\"transactionId\", \"amount\", \"status\"],\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the transaction.\"\n    },\n    \"transactionRef\": {\n      \"type\": \"string\",\n      \"description\": \"The system-generated transaction reference number.\"\n    },\n    \"merchantTxRef\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant-provided transaction reference for idempotency and reconciliation.\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"The transaction amount.\",\n      \"minimum\":\
  \ 0\n    },\n    \"fee\": {\n      \"type\": \"number\",\n      \"description\": \"The fee charged for the transaction.\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"The ISO 4217 currency code for the transaction.\",\n      \"pattern\": \"^[A-Z]{3}$\",\n      \"example\": \"NGN\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The transaction type indicating the direction of funds.\",\n      \"enum\": [\"credit\", \"debit\"]\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The channel through which the transaction was initiated.\",\n      \"enum\": [\"pos\", \"web\", \"app\", \"api\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the transaction.\",\n      \"enum\": [\"successful\", \"pending\", \"failed\", \"reversed\"]\n    },\n    \"terminalId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The POS terminal identifier, present for terminal-based transactions.\"\n    },\n    \"rrn\": {\n      \"type\": \"string\",\n      \"description\": \"The Retrieval Reference Number for POS transactions.\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"The session identifier linking related transaction steps.\"\n    },\n    \"narration\": {\n      \"type\": \"string\",\n      \"description\": \"A description or note associated with the transaction.\",\n      \"maxLength\": 200\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the transaction was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the transaction was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/json-schema/nomba-transaction-schema.json
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
title: Nomba Transaction
---
