---
description: A registered payment beneficiary
layout: schema
name: Beneficiary
properties_list:
- description: Unique beneficiary identifier
  name: beneficiaryId
  type: string
- description: Owning customer identifier
  name: customerId
  type: string
- description: Name of the beneficiary
  name: beneficiaryName
  type: string
- description: Beneficiary account number
  name: accountNumber
  type: string
- description: Beneficiary IBAN
  name: iban
  type: string
- description: Beneficiary bank BIC/SWIFT code
  name: bic
  type: string
- description: Name of the beneficiary bank
  name: bankName
  type: string
- description: Country of the beneficiary bank
  name: bankCountry
  type: string
- description: Default payment currency
  name: currency
  type: string
- description: Type of beneficiary
  name: beneficiaryType
  type: string
- description: Beneficiary status
  name: status
  type: string
- description: User-defined nickname for the beneficiary
  name: nickname
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-beneficiary-schema.json
slug: temenos-transact-core-banking-beneficiary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Beneficiary\",\n  \"type\": \"object\",\n  \"description\": \"A registered payment beneficiary\",\n  \"properties\": {\n    \"beneficiaryId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique beneficiary identifier\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Owning customer identifier\"\n    },\n    \"beneficiaryName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the beneficiary\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary account number\"\n    },\n    \"iban\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary IBAN\"\n    },\n    \"bic\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary bank BIC/SWIFT code\"\n    },\n    \"bankName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the beneficiary bank\"\
  \n    },\n    \"bankCountry\": {\n      \"type\": \"string\",\n      \"description\": \"Country of the beneficiary bank\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Default payment currency\"\n    },\n    \"beneficiaryType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of beneficiary\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Beneficiary status\"\n    },\n    \"nickname\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined nickname for the beneficiary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-beneficiary-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Beneficiary
---
