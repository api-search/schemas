---
description: Payment beneficiary details
layout: schema
name: Beneficiary
properties_list:
- description: Beneficiary name
  name: name
  type: string
- description: Beneficiary account number
  name: accountNumber
  type: string
- description: Beneficiary bank routing number (ABA)
  name: routingNumber
  type: string
- description: Beneficiary bank name
  name: bankName
  type: string
- description: Beneficiary bank address
  name: bankAddress
  type: string
- description: SWIFT/BIC code for international wires
  name: swiftCode
  type: string
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/beneficiary-schema.json
slug: beneficiary
source_filename: beneficiary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/beneficiary-schema.json\",\n  \"title\": \"Beneficiary\",\n  \"type\": \"object\",\n  \"description\": \"Payment beneficiary details\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary name\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary account number\"\n    },\n    \"routingNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary bank routing number (ABA)\"\n    },\n    \"bankName\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary bank name\"\n    },\n    \"bankAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary bank address\"\n    },\n    \"swiftCode\": {\n      \"type\": \"string\",\n      \"description\": \"SWIFT/BIC code for international wires\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/beneficiary-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Beneficiary
---
