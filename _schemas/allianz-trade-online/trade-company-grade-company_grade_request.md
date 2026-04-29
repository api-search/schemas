---
description: Request body for requesting a company creditworthiness grade
layout: schema
name: CompanyGradeRequest
properties_list:
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Name of the company to grade
  name: companyName
  type: string
- description: Official company registration number
  name: companyRegistrationNumber
  type: string
- description: ISO 3166-1 alpha-2 country code of the company
  name: country
  type: string
- description: Requested credit limit amount
  name: requestedCreditLimit
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-company-grade-company_grade_request-schema.json
slug: trade-company-grade-company_grade_request
source_filename: trade-company-grade-company_grade_request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-company-grade-company_grade_request-schema.json\",\n  \"title\": \"CompanyGradeRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for requesting a company creditworthiness grade\",\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the company to grade\"\n    },\n    \"companyRegistrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Official company registration number\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code of the company\"\n    },\n    \"requestedCreditLimit\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Requested\
  \ credit limit amount\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    }\n  },\n  \"required\": [\n    \"policyId\",\n    \"companyName\",\n    \"country\",\n    \"requestedCreditLimit\",\n    \"currency\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-company-grade-company_grade_request-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: CompanyGradeRequest
---
