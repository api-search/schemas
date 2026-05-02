---
description: A financial transaction entry on an account, aligned with ISO 20022 camt.053 (BankToCustomerStatement) entry structures. Represents a single credit or debit entry resulting from payment processing through Montran's infrastructure.
layout: schema
name: Montran Transaction
properties_list:
- description: Unique transaction identifier
  name: transactionId
  type: string
- description: Entry reference assigned by the account servicer
  name: entryReference
  type: string
- description: End-to-end identification from the originating payment
  name: endToEndId
  type: string
- description: Transaction amount
  name: amount
  type: number
- description: Transaction currency (ISO 4217)
  name: currency
  type: string
- description: Indicates whether the entry is a credit or debit
  name: creditDebitIndicator
  type: string
- description: Entry booking status
  name: status
  type: string
- description: Date when the entry was booked
  name: bookingDate
  type: string
- description: Value date of the entry
  name: valueDate
  type: string
- description: Name of the debtor
  name: debtorName
  type: string
- description: Debtor account identification
  name: debtorAccount
  type: object
- description: Name of the creditor
  name: creditorName
  type: string
- description: Creditor account identification
  name: creditorAccount
  type: object
- description: Remittance information or payment reference
  name: remittanceInformation
  type: string
- description: Bank transaction code identifying the type of transaction (ISO 20022 BankTransactionCode)
  name: bankTransactionCode
  type: object
- description: Proprietary bank transaction code
  name: proprietaryCode
  type: string
provider_name: Montran
provider_slug: montran
schema_file: json-schema/montran-transaction-schema.json
slug: montran-transaction
source_filename: montran-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.montran.com/schemas/transaction.json\",\n  \"title\": \"Montran Transaction\",\n  \"description\": \"A financial transaction entry on an account, aligned with ISO 20022 camt.053 (BankToCustomerStatement) entry structures. Represents a single credit or debit entry resulting from payment processing through Montran's infrastructure.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"transactionId\",\n    \"amount\",\n    \"currency\",\n    \"creditDebitIndicator\",\n    \"bookingDate\"\n  ],\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique transaction identifier\"\n    },\n    \"entryReference\": {\n      \"type\": \"string\",\n      \"description\": \"Entry reference assigned by the account servicer\"\n    },\n    \"endToEndId\": {\n      \"type\": \"string\",\n      \"description\": \"End-to-end identification from the originating\
  \ payment\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Transaction amount\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction currency (ISO 4217)\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"creditDebitIndicator\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the entry is a credit or debit\",\n      \"enum\": [\n        \"CRDT\",\n        \"DBIT\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Entry booking status\",\n      \"enum\": [\n        \"BOOK\",\n        \"PDNG\",\n        \"INFO\"\n      ]\n    },\n    \"bookingDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the entry was booked\"\n    },\n    \"valueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Value date of the entry\"\n    },\n    \"\
  debtorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the debtor\"\n    },\n    \"debtorAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Debtor account identification\",\n      \"properties\": {\n        \"iban\": {\n          \"type\": \"string\"\n        },\n        \"accountNumber\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"creditorName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the creditor\"\n    },\n    \"creditorAccount\": {\n      \"type\": \"object\",\n      \"description\": \"Creditor account identification\",\n      \"properties\": {\n        \"iban\": {\n          \"type\": \"string\"\n        },\n        \"accountNumber\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"remittanceInformation\": {\n      \"type\": \"string\",\n      \"description\": \"Remittance information or payment reference\"\n    },\n    \"bankTransactionCode\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Bank transaction code identifying the type of transaction (ISO 20022 BankTransactionCode)\",\n      \"properties\": {\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Domain code (e.g., PMNT for Payments)\"\n        },\n        \"family\": {\n          \"type\": \"string\",\n          \"description\": \"Family code within the domain\"\n        },\n        \"subFamily\": {\n          \"type\": \"string\",\n          \"description\": \"Sub-family code\"\n        }\n      }\n    },\n    \"proprietaryCode\": {\n      \"type\": \"string\",\n      \"description\": \"Proprietary bank transaction code\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/montran/refs/heads/main/json-schema/montran-transaction-schema.json
tags:
- Banking
- Central Banking
- Financial Services
- ISO 20022
- Market Infrastructure
- Messaging
- Payments
- Real-Time Payments
- SWIFT
title: Montran Transaction
---
