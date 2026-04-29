---
description: ''
layout: schema
name: Update1
properties_list:
- description: ''
  name: giftCommitmentId
  type: string
- description: ''
  name: paymentInstrument
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update1-schema.json
slug: salesforce-update1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"giftCommitmentId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"paymentInstrument\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"accountHolderName\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"last4\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardBrand\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\
  \n        },\n        \"digitalWalletProvider\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"bankAccountHolderType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountType\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankAccountNumber\": {\n          \"type\": \"string\",\n          \"example\": 42\n        },\n        \"bankCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"processorPaymentReference\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"gatewayReference\": {\n          \"type\": \"string\",\n \
  \         \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"accountHolderName\",\n        \"expiryMonth\",\n        \"expiryYear\",\n        \"last4\",\n        \"cardBrand\",\n        \"bankName\",\n        \"digitalWalletProvider\",\n        \"bankAccountHolderType\",\n        \"bankAccountType\",\n        \"bankAccountNumber\",\n        \"bankCode\",\n        \"gatewayName\",\n        \"processorName\",\n        \"processorPaymentReference\",\n        \"gatewayReference\"\n      ]\n    }\n  },\n  \"required\": [\n    \"giftCommitmentId\",\n    \"paymentInstrument\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Update1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update1-schema.json
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
title: Update1
---
