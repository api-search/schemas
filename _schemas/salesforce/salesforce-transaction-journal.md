---
description: ''
layout: schema
name: TransactionJournal
properties_list:
- description: ''
  name: activityDate
  type: string
- description: ''
  name: journalSubType
  type: string
- description: ''
  name: journalType
  type: string
- description: ''
  name: loyaltyProgram
  type: string
- description: ''
  name: loyaltyProgramMember
  type: string
- description: ''
  name: referredMember
  type: '[''string'', ''null'']'
- description: ''
  name: status
  type: string
- description: ''
  name: transactionJournalId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-journal-schema.json
slug: salesforce-transaction-journal
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"journalSubType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"journalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyProgram\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"loyaltyProgramMember\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"referredMember\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"transactionJournalId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"activityDate\",\n    \"journalSubType\",\n    \"journalType\",\n    \"loyaltyProgram\",\n\
  \    \"loyaltyProgramMember\",\n    \"referredMember\",\n    \"status\",\n    \"transactionJournalId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionJournal\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-journal-schema.json
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
title: TransactionJournal
---
