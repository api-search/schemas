---
description: ''
layout: schema
name: JournalLine
properties_list:
- description: Journal line number
  name: jeLineNum
  type: integer
- description: Chart of accounts code combination identifier
  name: codeCombinatonId
  type: integer
- description: Debit amount in functional currency
  name: accountedDr
  type: number
- description: Credit amount in functional currency
  name: accountedCr
  type: number
- description: Debit amount in entered currency
  name: enteredDr
  type: number
- description: Credit amount in entered currency
  name: enteredCr
  type: number
- description: Line description
  name: description
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-journal-line-schema.json
slug: financial-services-journal-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jeLineNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Journal line number\"\n    },\n    \"codeCombinatonId\": {\n      \"type\": \"integer\",\n      \"description\": \"Chart of accounts code combination identifier\"\n    },\n    \"accountedDr\": {\n      \"type\": \"number\",\n      \"description\": \"Debit amount in functional currency\"\n    },\n    \"accountedCr\": {\n      \"type\": \"number\",\n      \"description\": \"Credit amount in functional currency\"\n    },\n    \"enteredDr\": {\n      \"type\": \"number\",\n      \"description\": \"Debit amount in entered currency\"\n    },\n    \"enteredCr\": {\n      \"type\": \"number\",\n      \"description\": \"Credit amount in entered currency\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Line description\"\n  \
  \  }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-journal-line-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: JournalLine
---
