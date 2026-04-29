---
description: ''
layout: schema
name: Update
properties_list:
- description: ''
  name: giftTransactionId
  type: string
- description: ''
  name: transactionStatus
  type: string
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
- description: ''
  name: processorTransactionFee
  type: number
- description: ''
  name: gatewayTransactionFee
  type: number
- description: ''
  name: donorCoverAmount
  type: number
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-schema.json
slug: salesforce-update
source_filename: salesforce-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"giftTransactionId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"transactionStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"processorReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayResponseCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayErrorMessage\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastGatewayProcessedDateTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"processorTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"gatewayTransactionFee\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n\
  \    },\n    \"donorCoverAmount\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    }\n  },\n  \"required\": [\n    \"giftTransactionId\",\n    \"transactionStatus\",\n    \"processorReference\",\n    \"gatewayReference\",\n    \"lastGatewayResponseCode\",\n    \"lastGatewayErrorMessage\",\n    \"lastGatewayProcessedDateTime\",\n    \"processorTransactionFee\",\n    \"gatewayTransactionFee\",\n    \"donorCoverAmount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Update\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-schema.json
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
title: Update
---
