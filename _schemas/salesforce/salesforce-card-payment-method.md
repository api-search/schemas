---
description: ''
layout: schema
name: CardPaymentMethod
properties_list:
- description: ''
  name: cardHolderName
  type: string
- description: ''
  name: expiryMonth
  type: string
- description: ''
  name: expiryYear
  type: string
- description: ''
  name: cardNumber
  type: string
- description: ''
  name: cvv
  type: string
- description: ''
  name: cardCategory
  type: string
- description: ''
  name: cardType
  type: string
- description: ''
  name: startYear
  type: string
- description: ''
  name: startMonth
  type: string
- description: ''
  name: nickName
  type: string
- description: ''
  name: accountId
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-card-payment-method-schema.json
slug: salesforce-card-payment-method
source_filename: salesforce-card-payment-method-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardHolderName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"expiryMonth\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"expiryYear\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cardNumber\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cvv\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cardCategory\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cardType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"startYear\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"startMonth\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"nickName\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"example_value\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"cardHolderName\",\n    \"expiryMonth\",\n    \"expiryYear\",\n    \"cardNumber\",\n    \"cvv\",\n    \"cardCategory\",\n    \"cardType\",\n    \"startYear\",\n    \"startMonth\",\n    \"nickName\",\n    \"accountId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CardPaymentMethod\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-card-payment-method-schema.json
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
title: CardPaymentMethod
---
