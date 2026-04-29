---
description: ''
layout: schema
name: JournalEntryLine
properties_list:
- description: General ledger account code
  name: AccountCode
  type: string
- description: Debit amount in local currency
  name: Debit
  type: number
- description: Credit amount in local currency
  name: Credit
  type: number
- description: Short name or business partner code
  name: ShortName
  type: string
- description: Memo for this line
  name: LineMemo
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-journal-entry-line-schema.json
slug: sap-business-one-service-layer-journal-entry-line
source_filename: sap-business-one-service-layer-journal-entry-line-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalEntryLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountCode\": {\n      \"type\": \"string\",\n      \"description\": \"General ledger account code\"\n    },\n    \"Debit\": {\n      \"type\": \"number\",\n      \"description\": \"Debit amount in local currency\"\n    },\n    \"Credit\": {\n      \"type\": \"number\",\n      \"description\": \"Credit amount in local currency\"\n    },\n    \"ShortName\": {\n      \"type\": \"string\",\n      \"description\": \"Short name or business partner code\"\n    },\n    \"LineMemo\": {\n      \"type\": \"string\",\n      \"description\": \"Memo for this line\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-journal-entry-line-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: JournalEntryLine
---
