---
description: ''
layout: schema
name: TransactionLedgerSummary
properties_list:
- description: ''
  name: message
  type: '[''string'', ''null'']'
- description: ''
  name: status
  type: boolean
- description: ''
  name: transactionJournalCount
  type: integer
- description: ''
  name: transactionJournals
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-ledger-summary-schema.json
slug: salesforce-transaction-ledger-summary
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"transactionJournalCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"transactionJournals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"activityDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"additionalTransactionJournalAttributes\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"journalSubTypeName\": {\n            \"type\": \"string\",\n            \"example\"\
  : \"example_value\"\n          },\n          \"journalTypeName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"pointsChange\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"transactionJournalId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"transactionJournalNumber\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"activityDate\",\n          \"additionalTransactionJournalAttributes\",\n          \"journalSubTypeName\",\n          \"journalTypeName\",\n          \"pointsChange\",\n          \"transactionJournalId\",\n          \"transactionJournalNumber\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\
  ,\n    \"status\",\n    \"transactionJournalCount\",\n    \"transactionJournals\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionLedgerSummary\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-ledger-summary-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: TransactionLedgerSummary
---
