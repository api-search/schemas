---
description: ''
layout: schema
name: AccountingJournal
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: journalNumber
  type: string
- description: ''
  name: accountingDate
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: totalDebitAmount
  type: number
- description: ''
  name: totalCreditAmount
  type: number
provider_name: Workday
provider_slug: workday
schema_file: json-schema/financialManagement-accounting-journal-schema.json
slug: financialManagement-accounting-journal
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountingJournal\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"journalNumber\": {\n      \"type\": \"string\"\n    },\n    \"accountingDate\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"totalDebitAmount\": {\n      \"type\": \"number\"\n    },\n    \"totalCreditAmount\": {\n      \"type\": \"number\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/financialManagement-accounting-journal-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: AccountingJournal
---
