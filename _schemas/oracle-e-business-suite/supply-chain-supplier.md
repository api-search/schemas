---
description: ''
layout: schema
name: Supplier
properties_list:
- description: Vendor identifier
  name: vendorId
  type: integer
- description: Vendor name
  name: vendorName
  type: string
- description: Vendor number
  name: segment1
  type: string
- description: Vendor type lookup code
  name: vendorType
  type: string
- description: Tax payer identification number
  name: taxPayerId
  type: string
- description: Standard industry classification
  name: standardIndustryClass
  type: string
- description: Default payment currency
  name: paymentCurrencyCode
  type: string
- description: Default payment method
  name: paymentMethodCode
  type: string
- description: Default payment terms identifier
  name: termsId
  type: integer
- description: Whether the vendor is active
  name: enabled
  type: boolean
- description: ''
  name: startDateActive
  type: string
- description: ''
  name: endDateActive
  type: string
- description: ''
  name: sites
  type: array
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/supply-chain-supplier-schema.json
slug: supply-chain-supplier
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Supplier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vendorId\": {\n      \"type\": \"integer\",\n      \"description\": \"Vendor identifier\"\n    },\n    \"vendorName\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor name\"\n    },\n    \"segment1\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor number\"\n    },\n    \"vendorType\": {\n      \"type\": \"string\",\n      \"description\": \"Vendor type lookup code\"\n    },\n    \"taxPayerId\": {\n      \"type\": \"string\",\n      \"description\": \"Tax payer identification number\"\n    },\n    \"standardIndustryClass\": {\n      \"type\": \"string\",\n      \"description\": \"Standard industry classification\"\n    },\n    \"paymentCurrencyCode\": {\n      \"type\": \"string\",\n      \"description\": \"Default payment currency\"\n    },\n    \"paymentMethodCode\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Default payment method\"\n    },\n    \"termsId\": {\n      \"type\": \"integer\",\n      \"description\": \"Default payment terms identifier\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the vendor is active\"\n    },\n    \"startDateActive\": {\n      \"type\": \"string\"\n    },\n    \"endDateActive\": {\n      \"type\": \"string\"\n    },\n    \"sites\": {\n      \"type\": \"array\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/supply-chain-supplier-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: Supplier
---
