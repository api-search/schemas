---
description: ''
layout: schema
name: ProcessParameter1
properties_list:
- description: ''
  name: TransactionJournal
  type: object
- description: ''
  name: PointsToCredit
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-process-parameter1-schema.json
slug: salesforce-process-parameter1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransactionJournal\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ActivityDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"ExternalTransactionNumber\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"InvoiceDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"JournalTypeName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"MembershipNumber\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"TransactionAmount\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"CurrencyIsoCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"Status\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"ActivityDate\",\n        \"ExternalTransactionNumber\",\n        \"InvoiceDate\",\n        \"JournalTypeName\",\n        \"MembershipNumber\",\n        \"TransactionAmount\",\n        \"CurrencyIsoCode\",\n        \"Status\"\n      ]\n    },\n    \"PointsToCredit\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"TransactionJournal\",\n    \"PointsToCredit\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessParameter1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-process-parameter1-schema.json
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
title: ProcessParameter1
---
