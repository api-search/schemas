---
description: ''
layout: schema
name: GeneralLedgerEntry
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: entryNumber
  type: integer
- description: ''
  name: postingDate
  type: string
- description: ''
  name: documentNumber
  type: string
- description: ''
  name: documentType
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: debitAmount
  type: number
- description: ''
  name: creditAmount
  type: number
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-general-ledger-entry-schema.json
slug: business-central-v2-general-ledger-entry
source_filename: business-central-v2-general-ledger-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GeneralLedgerEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"entryNumber\": {\n      \"type\": \"integer\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\"\n    },\n    \"documentNumber\": {\n      \"type\": \"string\"\n    },\n    \"documentType\": {\n      \"type\": \"string\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"debitAmount\": {\n      \"type\": \"number\"\n    },\n    \"creditAmount\": {\n      \"type\": \"number\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-general-ledger-entry-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: GeneralLedgerEntry
---
