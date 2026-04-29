---
description: ''
layout: schema
name: CreatePaymentMethodRequest
properties_list:
- description: ''
  name: paymentGatewayId
  type: string
- description: ''
  name: cardPaymentMethod
  type: object
- description: ''
  name: phone
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: additionalData
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-payment-method-request-schema.json
slug: salesforce-create-payment-method-request
source_filename: salesforce-create-payment-method-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"paymentGatewayId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"cardPaymentMethod\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cardHolderName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"expiryYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardNumber\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cvv\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardCategory\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"cardType\": {\n          \"type\": \"string\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"startYear\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"startMonth\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"nickName\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"accountId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"cardHolderName\",\n        \"expiryMonth\",\n        \"expiryYear\",\n        \"cardNumber\",\n        \"cvv\",\n        \"cardCategory\",\n        \"cardType\",\n        \"startYear\",\n        \"startMonth\",\n        \"nickName\",\n        \"accountId\"\n      ]\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"additionalData\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"key1\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"key2\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"key1\",\n        \"key2\"\n      ]\n    }\n  },\n  \"required\": [\n    \"paymentGatewayId\",\n    \"cardPaymentMethod\",\n    \"phone\",\n    \"email\",\n    \"additionalData\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreatePaymentMethodRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-payment-method-request-schema.json
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
title: CreatePaymentMethodRequest
---
