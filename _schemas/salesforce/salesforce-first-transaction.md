---
description: ''
layout: schema
name: FirstTransaction
properties_list:
- description: ''
  name: amount
  type: number
- description: ''
  name: receivedDate
  type: string
- description: ''
  name: donorCoverAmount
  type: number
- description: ''
  name: transactionStatus
  type: string
- description: ''
  name: gatewayTransactionFee
  type: number
- description: ''
  name: processorTransactionFee
  type: number
- description: ''
  name: processorReference
  type: string
- description: ''
  name: gatewayReference
  type: string
- description: ''
  name: lastGatewayResponseCode
  type: string
- description: ''
  name: lastGatewayErrorMessage
  type: string
- description: ''
  name: lastGatewayProcessedDateTime
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-first-transaction-schema.json
slug: salesforce-first-transaction
source_filename: salesforce-first-transaction-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"amount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"receivedDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"donorCoverAmount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"transactionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"processorTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"processorReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayResponseCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayErrorMessage\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayProcessedDateTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"amount\",\n    \"receivedDate\",\n    \"donorCoverAmount\",\n    \"transactionStatus\",\n    \"gatewayTransactionFee\",\n    \"processorTransactionFee\",\n    \"processorReference\",\n    \"gatewayReference\",\n    \"lastGatewayResponseCode\",\n    \"lastGatewayErrorMessage\",\n    \"lastGatewayProcessedDateTime\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FirstTransaction\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-first-transaction-schema.json
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
title: FirstTransaction
---
