---
description: An account statement
layout: schema
name: Statement
properties_list:
- description: Unique statement identifier
  name: statementId
  type: string
- description: Associated account ID
  name: accountId
  type: string
- description: Statement date
  name: statementDate
  type: string
- description: ''
  name: openingBalance
  type: number
- description: ''
  name: closingBalance
  type: number
- description: ''
  name: currency
  type: string
- description: ''
  name: totalCredits
  type: number
- description: ''
  name: totalDebits
  type: number
- description: ''
  name: transactionCount
  type: integer
provider_name: Bank of America
provider_slug: bank-of-america
schema_file: json-schema/statement-schema.json
slug: statement
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/bank-of-america/json-schema/statement-schema.json\",\n  \"title\": \"Statement\",\n  \"type\": \"object\",\n  \"description\": \"An account statement\",\n  \"properties\": {\n    \"statementId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique statement identifier\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated account ID\"\n    },\n    \"statementDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Statement date\"\n    },\n    \"openingBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"closingBalance\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"currency\": {\n      \"type\": \"string\"\n    },\n    \"totalCredits\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n\
  \    \"totalDebits\": {\n      \"type\": \"number\",\n      \"format\": \"double\"\n    },\n    \"transactionCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bank-of-america/refs/heads/main/json-schema/statement-schema.json
tags:
- Banking
- Corporate Banking
- Finance
- Payments
- Treasury
- CashPro
title: Statement
---
