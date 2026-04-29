---
description: Contains the a single or dual message transaction identifier values used for searching the respective transaction. Acquirer Reference Number, Banknet Reference Number, Trace Id and Serial Id values are captured.
layout: schema
name: TransactionIdentifier
properties_list:
- description: Contains Acquirer Reference Number for a transaction.
  name: acqRefNum
  type: string
- description: Contains Banknet Reference Number for a transaction.
  name: banknetRefNum
  type: string
- description: Contains Trace Id for a transaction.
  name: traceId
  type: string
- description: Contains Serial Id for a transaction.
  name: serialId
  type: string
provider_name: Mastercard
provider_slug: mastercard
schema_file: json-schema/mastercard-suspected-fraud-transaction-identifier-schema.json
slug: mastercard-suspected-fraud-transaction-identifier
source_filename: mastercard-suspected-fraud-transaction-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionIdentifier\",\n  \"type\": \"object\",\n  \"description\": \"Contains the a single or dual message transaction identifier values used for searching the respective transaction. Acquirer Reference Number, Banknet Reference Number, Trace Id and Serial Id values are captured.\",\n  \"properties\": {\n    \"acqRefNum\": {\n      \"type\": \"string\",\n      \"description\": \"Contains Acquirer Reference Number for a transaction.\"\n    },\n    \"banknetRefNum\": {\n      \"type\": \"string\",\n      \"description\": \"Contains Banknet Reference Number for a transaction.\"\n    },\n    \"traceId\": {\n      \"type\": \"string\",\n      \"description\": \"Contains Trace Id  for a transaction.\"\n    },\n    \"serialId\": {\n      \"type\": \"string\",\n      \"description\": \"Contains Serial Id for a transaction.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mastercard/refs/heads/main/json-schema/mastercard-suspected-fraud-transaction-identifier-schema.json
tags:
- Credit Cards
- Digital Identity
- Financial Services
- Fraud Detection
- Open Banking
- Payments
title: TransactionIdentifier
---
