---
description: A company creditworthiness grade from Allianz Trade
layout: schema
name: CompanyGrade
properties_list:
- description: Unique identifier for the company grade
  name: gradeId
  type: string
- description: Trade credit insurance policy identifier
  name: policyId
  type: string
- description: Name of the graded company
  name: companyName
  type: string
- description: Official company registration number
  name: companyRegistrationNumber
  type: string
- description: ISO 3166-1 alpha-2 country code
  name: country
  type: string
- description: Creditworthiness grade letter
  name: grade
  type: string
- description: Numeric score underlying the grade (0-100)
  name: gradeScore
  type: integer
- description: ISO 4217 currency code
  name: currency
  type: string
- description: Approved credit limit amount
  name: creditLimit
  type: number
- description: Originally requested credit limit
  name: requestedCreditLimit
  type: number
- description: Date until which the grade is valid
  name: validUntil
  type: string
- description: Timestamp when the grade was issued
  name: gradedAt
  type: string
provider_name: Allianz Trade
provider_slug: allianz-trade-online
schema_file: json-schema/trade-company-grade-company_grade-schema.json
slug: trade-company-grade-company_grade
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.allianz-trade.com/schemas/trade-company-grade-company_grade-schema.json\",\n  \"title\": \"CompanyGrade\",\n  \"type\": \"object\",\n  \"description\": \"A company creditworthiness grade from Allianz Trade\",\n  \"properties\": {\n    \"gradeId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the company grade\"\n    },\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Trade credit insurance policy identifier\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the graded company\"\n    },\n    \"companyRegistrationNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Official company registration number\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code\"\n    },\n    \"grade\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Creditworthiness grade letter\",\n      \"enum\": [\n        \"A\",\n        \"B\",\n        \"C\",\n        \"D\",\n        \"E\"\n      ]\n    },\n    \"gradeScore\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric score underlying the grade (0-100)\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\"\n    },\n    \"creditLimit\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Approved credit limit amount\"\n    },\n    \"requestedCreditLimit\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Originally requested credit limit\"\n    },\n    \"validUntil\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date until which the grade is valid\"\n    },\n    \"gradedAt\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"Timestamp when the grade was issued\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/json-schema/trade-company-grade-company_grade-schema.json
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
title: CompanyGrade
---
