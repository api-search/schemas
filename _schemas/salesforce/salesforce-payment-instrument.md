---
description: ''
layout: schema
name: PaymentInstrument
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: accountHolderName
  type: string
- description: ''
  name: expiryMonth
  type: string
- description: ''
  name: expiryYear
  type: string
- description: ''
  name: last4
  type: string
- description: ''
  name: cardBrand
  type: string
- description: ''
  name: bankName
  type: string
- description: ''
  name: digitalWalletProvider
  type: string
- description: ''
  name: bankAccountHolderType
  type: string
- description: ''
  name: bankAccountType
  type: string
- description: ''
  name: bankAccountNumber
  type: string
- description: ''
  name: bankCode
  type: string
- description: ''
  name: gatewayName
  type: string
- description: ''
  name: processorName
  type: string
- description: ''
  name: processorPaymentReference
  type: string
- description: ''
  name: gatewayReference
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-payment-instrument-schema.json
slug: salesforce-payment-instrument
source_filename: salesforce-payment-instrument-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"accountHolderName\": {\n      \"type\": \"string\",\n      \"example\": 42\n    },\n    \"expiryMonth\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"expiryYear\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"last4\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cardBrand\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"bankName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"digitalWalletProvider\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"bankAccountHolderType\": {\n      \"type\": \"string\",\n      \"example\": 42\n    },\n    \"bankAccountType\": {\n      \"type\": \"string\",\n      \"example\"\
  : 42\n    },\n    \"bankAccountNumber\": {\n      \"type\": \"string\",\n      \"example\": 42\n    },\n    \"bankCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"processorName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"processorPaymentReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"gatewayReference\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"accountHolderName\",\n    \"expiryMonth\",\n    \"expiryYear\",\n    \"last4\",\n    \"cardBrand\",\n    \"bankName\",\n    \"digitalWalletProvider\",\n    \"bankAccountHolderType\",\n    \"bankAccountType\",\n    \"bankAccountNumber\",\n    \"bankCode\",\n    \"gatewayName\",\n    \"processorName\",\n    \"processorPaymentReference\",\n\
  \    \"gatewayReference\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaymentInstrument\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-payment-instrument-schema.json
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
title: PaymentInstrument
---
