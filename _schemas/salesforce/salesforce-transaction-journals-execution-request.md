---
description: ''
layout: schema
name: TransactionJournalsExecutionRequest
properties_list:
- description: ''
  name: transactionJournals
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-transaction-journals-execution-request-schema.json
slug: salesforce-transaction-journals-execution-request
source_filename: salesforce-transaction-journals-execution-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionJournals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ActivityDate\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"JournalTypeId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"LoyaltyProgramId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"MemberId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"Status\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"appliedPromotions\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\"\
  : {\n              \"type\": \"object\",\n              \"properties\": {\n                \"promotionId\": {\n                  \"type\": \"string\",\n                  \"example\": \"500123\"\n                },\n                \"rewards\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                }\n              },\n              \"required\": [\n                \"promotionId\",\n                \"rewards\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"ActivityDate\",\n          \"JournalTypeId\",\n          \"LoyaltyProgramId\",\n          \"MemberId\",\n          \"Status\",\n          \"appliedPromotions\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"transactionJournals\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n\
  \  \"title\": \"TransactionJournalsExecutionRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-transaction-journals-execution-request-schema.json
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
title: TransactionJournalsExecutionRequest
---
