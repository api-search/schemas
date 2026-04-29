---
description: ''
layout: schema
name: CreditPointstoMembersRequest
properties_list:
- description: ''
  name: processParameters
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-credit-pointsto-members-request-schema.json
slug: salesforce-credit-pointsto-members-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"processParameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"TransactionJournal\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ActivityDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"ExternalTransactionNumber\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"InvoiceDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"JournalTypeName\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"MembershipNumber\": {\n                \"type\": \"string\"\
  ,\n                \"example\": \"example_value\"\n              },\n              \"TransactionAmount\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"CurrencyIsoCode\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"Status\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            },\n            \"required\": [\n              \"ActivityDate\",\n              \"ExternalTransactionNumber\",\n              \"InvoiceDate\",\n              \"JournalTypeName\",\n              \"MembershipNumber\",\n              \"TransactionAmount\",\n              \"CurrencyIsoCode\",\n              \"Status\"\n            ]\n          },\n          \"PointsToCredit\": {\n            \"type\": \"number\",\n            \"example\": 42.5\n          }\n        },\n        \"required\": [\n  \
  \        \"TransactionJournal\",\n          \"PointsToCredit\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"processParameters\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreditPointstoMembersRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-credit-pointsto-members-request-schema.json
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
title: CreditPointstoMembersRequest
---
