---
description: ''
layout: schema
name: TransactionJournalsSimulationRequest
properties_list:
- description: ''
  name: transactionJournals
  type: array
- description: ''
  name: runSetting
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-journals-simulation-request-schema.json
slug: salesforce-transaction-journals-simulation-request
source_filename: salesforce-transaction-journals-simulation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionJournals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"CurrencyIsoCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"ActivityDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"JournalDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Brand\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Establishment\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"ExternalTransactionNumber\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n       \
  \   },\n          \"JournalTypeId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"LoyaltyProgramId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"MemberId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"TransactionAmount\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"TransactionLocation\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"VoucherCode\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Origin\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Distance\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Destination\"\
  : {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"FlightNumber\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"CurrencyIsoCode\",\n          \"ActivityDate\",\n          \"JournalDate\",\n          \"Brand\",\n          \"Establishment\",\n          \"ExternalTransactionNumber\",\n          \"JournalTypeId\",\n          \"LoyaltyProgramId\",\n          \"MemberId\",\n          \"TransactionAmount\",\n          \"TransactionLocation\",\n          \"VoucherCode\",\n          \"Origin\",\n          \"Distance\",\n          \"Destination\",\n          \"FlightNumber\",\n          \"Status\"\n        ]\n      }\n    },\n    \"runSetting\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isSimulation\"\
  : {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"isSimulation\"\n      ]\n    }\n  },\n  \"required\": [\n    \"transactionJournals\",\n    \"runSetting\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TransactionJournalsSimulationRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-journals-simulation-request-schema.json
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
title: TransactionJournalsSimulationRequest
---
