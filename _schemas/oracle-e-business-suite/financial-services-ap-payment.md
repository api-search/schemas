---
description: ''
layout: schema
name: ApPayment
properties_list:
- description: Payment check identifier
  name: checkId
  type: integer
- description: Check number
  name: checkNumber
  type: integer
- description: Payment amount
  name: amount
  type: number
- description: Payment currency code
  name: currencyCode
  type: string
- description: Check date
  name: checkDate
  type: string
- description: Vendor identifier
  name: vendorId
  type: integer
- description: Vendor name
  name: vendorName
  type: string
- description: Bank account identifier
  name: bankAccountId
  type: integer
- description: Payment method
  name: paymentMethodCode
  type: string
- description: Payment status
  name: status
  type: string
- description: ''
  name: orgId
  type: integer
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-ap-payment-schema.json
slug: financial-services-ap-payment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApPayment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"checkId\": {\n      \"type\": \"integer\",\n      \"description\": \"Payment check identifier\"\n    },\n    \"checkNumber\": {\n      \"type\": \"integer\",\n      \"description\": \"Check number\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Payment amount\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Payment currency code\"\n    },\n    \"checkDate\": {\n      \"type\": \"string\",\n      \"description\": \"Check date\"\n    },\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor identifier\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor name\"\n    },\n    \"bankAccountId\": {\n      \"type\": \"integer\",\n      \"description\": \"Bank account identifier\"\n    },\n\
  \    \"paymentMethodCode\": {\n      \"type\": \"string\",\n      \"description\": \"Payment method\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Payment status\"\n    },\n    \"orgId\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-ap-payment-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: ApPayment
---
