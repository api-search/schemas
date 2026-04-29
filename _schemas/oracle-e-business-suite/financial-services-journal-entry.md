---
description: ''
layout: schema
name: JournalEntry
properties_list:
- description: Journal entry header identifier
  name: jeHeaderId
  type: integer
- description: Journal batch identifier
  name: jeBatchId
  type: integer
- description: Ledger identifier
  name: ledgerId
  type: integer
- description: Accounting period name
  name: periodName
  type: string
- description: Journal entry name
  name: journalName
  type: string
- description: Journal category
  name: journalCategory
  type: string
- description: Journal source
  name: journalSource
  type: string
- description: Currency code (ISO 4217)
  name: currencyCode
  type: string
- description: Journal status
  name: status
  type: string
- description: Journal description
  name: description
  type: string
- description: Journal effective date
  name: effectiveDate
  type: string
- description: ''
  name: lines
  type: array
- description: ''
  name: createdBy
  type: integer
- description: ''
  name: creationDate
  type: string
- description: ''
  name: lastUpdatedBy
  type: integer
- description: ''
  name: lastUpdateDate
  type: string
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/financial-services-journal-entry-schema.json
slug: financial-services-journal-entry
source_filename: financial-services-journal-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jeHeaderId\": {\n      \"type\": \"integer\",\n      \"description\": \"Journal entry header identifier\"\n    },\n    \"jeBatchId\": {\n      \"type\": \"integer\",\n      \"description\": \"Journal batch identifier\"\n    },\n    \"ledgerId\": {\n      \"type\": \"integer\",\n      \"description\": \"Ledger identifier\"\n    },\n    \"periodName\": {\n      \"type\": \"string\",\n      \"description\": \"Accounting period name\"\n    },\n    \"journalName\": {\n      \"type\": \"string\",\n      \"description\": \"Journal entry name\"\n    },\n    \"journalCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Journal category\"\n    },\n    \"journalSource\": {\n      \"type\": \"string\",\n      \"description\": \"Journal source\"\n    },\n    \"currencyCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Currency code (ISO 4217)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Journal status\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Journal description\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"Journal effective date\"\n    },\n    \"lines\": {\n      \"type\": \"array\"\n    },\n    \"createdBy\": {\n      \"type\": \"integer\"\n    },\n    \"creationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdatedBy\": {\n      \"type\": \"integer\"\n    },\n    \"lastUpdateDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/financial-services-journal-entry-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: JournalEntry
---
