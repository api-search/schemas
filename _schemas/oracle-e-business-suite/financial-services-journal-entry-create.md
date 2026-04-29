---
description: ''
layout: schema
name: JournalEntryCreate
properties_list:
- description: ''
  name: ledgerId
  type: integer
- description: ''
  name: periodName
  type: string
- description: ''
  name: journalName
  type: string
- description: ''
  name: journalCategory
  type: string
- description: ''
  name: journalSource
  type: string
- description: ''
  name: currencyCode
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: lines
  type: array
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-journal-entry-create-schema.json
slug: financial-services-journal-entry-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalEntryCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ledgerId\": {\n      \"type\": \"integer\"\n    },\n    \"periodName\": {\n      \"type\": \"string\"\n    },\n    \"journalName\": {\n      \"type\": \"string\"\n    },\n    \"journalCategory\": {\n      \"type\": \"string\"\n    },\n    \"journalSource\": {\n      \"type\": \"string\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-journal-entry-create-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: JournalEntryCreate
---
