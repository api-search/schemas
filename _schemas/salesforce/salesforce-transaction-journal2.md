---
description: ''
layout: schema
name: TransactionJournal2
properties_list:
- description: ''
  name: activityDate
  type: string
- description: ''
  name: additionalTransactionJournalAttributes
  type: array
- description: ''
  name: journalSubTypeName
  type: string
- description: ''
  name: journalTypeName
  type: string
- description: ''
  name: pointsChange
  type: array
- description: ''
  name: transactionJournalId
  type: string
- description: ''
  name: transactionJournalNumber
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-journal2-schema.json
slug: salesforce-transaction-journal2
source_filename: salesforce-transaction-journal2-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"additionalTransactionJournalAttributes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"journalSubTypeName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"journalTypeName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"pointsChange\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"transactionJournalId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"transactionJournalNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"activityDate\"\
  ,\n    \"additionalTransactionJournalAttributes\",\n    \"journalSubTypeName\",\n    \"journalTypeName\",\n    \"pointsChange\",\n    \"transactionJournalId\",\n    \"transactionJournalNumber\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionJournal2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-journal2-schema.json
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
title: TransactionJournal2
---
