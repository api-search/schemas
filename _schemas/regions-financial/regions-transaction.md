---
description: A financial transaction on a Regions Bank account (FDX-compliant)
layout: schema
name: Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Account the transaction belongs to
  name: accountId
  type: string
- description: Date transaction was posted
  name: postedDate
  type: string
- description: Date transaction occurred
  name: transactionDate
  type: string
- description: Transaction amount (negative for debits)
  name: amount
  type: number
- description: ''
  name: currency
  type: string
- description: Transaction description text
  name: description
  type: string
- description: Spending category
  name: category
  type: string
- description: Transaction direction
  name: type
  type: string
- description: Transaction posting status
  name: status
  type: string
- description: Merchant name for card transactions
  name: merchantName
  type: string
- description: Merchant category code (MCC)
  name: merchantCategory
  type: string
provider_name: regions-financial
provider_slug: regions-financial
schema_file: json-schema/regions-transaction-schema.json
slug: regions-transaction
source_filename: regions-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regions-financial/json-schema/regions-transaction-schema.json\",\n  \"title\": \"Transaction\",\n  \"description\": \"A financial transaction on a Regions Bank account (FDX-compliant)\",\n  \"type\": \"object\",\n  \"required\": [\"transactionId\", \"accountId\", \"amount\", \"type\", \"status\"],\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Account the transaction belongs to\"\n    },\n    \"postedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date transaction was posted\"\n    },\n    \"transactionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date transaction occurred\"\n    },\n    \"amount\":\
  \ {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount (negative for debits)\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction description text\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Spending category\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"DEBIT\", \"CREDIT\"],\n      \"description\": \"Transaction direction\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"PENDING\", \"POSTED\"],\n      \"description\": \"Transaction posting status\"\n    },\n    \"merchantName\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant name for card transactions\"\n    },\n    \"merchantCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Merchant category code (MCC)\"\n    }\n  },\n  \"additionalProperties\"\
  : false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regions-financial/refs/heads/main/json-schema/regions-transaction-schema.json
tags:
- Banking
- Financial Services
- Open Banking
- FDX
- Consumer Banking
- Wealth Management
- Fortune 500
title: Transaction
---
