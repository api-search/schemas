---
description: ''
layout: schema
name: JournalEntry
properties_list:
- description: Journal entry number
  name: JdtNum
  type: integer
- description: Reference date
  name: ReferenceDate
  type: string
- description: Remark or memo for the journal entry
  name: Memo
  type: string
- description: Debit and credit lines
  name: JournalEntryLines
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-journal-entry-schema.json
slug: sap-business-one-service-layer-journal-entry
source_filename: sap-business-one-service-layer-journal-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JdtNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Journal entry number\"\n    },\n    \"ReferenceDate\": {\n      \"type\": \"string\",\n      \"description\": \"Reference date\"\n    },\n    \"Memo\": {\n      \"type\": \"string\",\n      \"description\": \"Remark or memo for the journal entry\"\n    },\n    \"JournalEntryLines\": {\n      \"type\": \"array\",\n      \"description\": \"Debit and credit lines\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-journal-entry-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: JournalEntry
---
