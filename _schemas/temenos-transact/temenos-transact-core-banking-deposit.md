---
description: A deposit arrangement in Temenos Transact
layout: schema
name: Deposit
properties_list:
- description: Unique deposit identifier
  name: depositId
  type: string
- description: Customer identifier
  name: customerId
  type: string
- description: Deposit product identifier
  name: productId
  type: string
- description: Name of the deposit product
  name: productName
  type: string
- description: Original deposit principal amount
  name: principalAmount
  type: number
- description: Current balance including accrued interest
  name: currentBalance
  type: number
- description: Deposit currency
  name: currency
  type: string
- description: Applied interest rate percentage
  name: interestRate
  type: number
- description: Interest accrued but not yet capitalized
  name: accruedInterest
  type: number
- description: Deposit start date
  name: startDate
  type: string
- description: Deposit maturity date
  name: maturityDate
  type: string
- description: Deposit term description
  name: term
  type: string
- description: Automatic renewal behaviour
  name: renewalType
  type: string
- description: Deposit status
  name: status
  type: string
provider_name: Temenos Transact
provider_slug: temenos-transact
schema_file: json-schema/temenos-transact-core-banking-deposit-schema.json
slug: temenos-transact-core-banking-deposit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deposit\",\n  \"type\": \"object\",\n  \"description\": \"A deposit arrangement in Temenos Transact\",\n  \"properties\": {\n    \"depositId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique deposit identifier\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"Customer identifier\"\n    },\n    \"productId\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit product identifier\"\n    },\n    \"productName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deposit product\"\n    },\n    \"principalAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Original deposit principal amount\"\n    },\n    \"currentBalance\": {\n      \"type\": \"number\",\n      \"description\": \"Current balance including accrued interest\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Deposit currency\"\n    },\n    \"interestRate\": {\n      \"type\": \"number\",\n      \"description\": \"Applied interest rate percentage\"\n    },\n    \"accruedInterest\": {\n      \"type\": \"number\",\n      \"description\": \"Interest accrued but not yet capitalized\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit start date\"\n    },\n    \"maturityDate\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit maturity date\"\n    },\n    \"term\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit term description\"\n    },\n    \"renewalType\": {\n      \"type\": \"string\",\n      \"description\": \"Automatic renewal behaviour\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Deposit status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos-transact/refs/heads/main/json-schema/temenos-transact-core-banking-deposit-schema.json
tags:
- Banking
- Core Banking
- Digital Banking
- Enterprise
- Financial Services
- Fintech
title: Deposit
---
