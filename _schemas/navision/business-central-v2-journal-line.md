---
description: ''
layout: schema
name: JournalLine
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: journalId
  type: string
- description: ''
  name: journalDisplayName
  type: string
- description: ''
  name: lineNumber
  type: integer
- description: ''
  name: accountType
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: accountNumber
  type: string
- description: ''
  name: postingDate
  type: string
- description: ''
  name: documentNumber
  type: string
- description: ''
  name: externalDocumentNumber
  type: string
- description: ''
  name: amount
  type: number
- description: ''
  name: description
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: taxCode
  type: string
- description: ''
  name: balanceAccountType
  type: string
- description: ''
  name: balanceAccountNumber
  type: string
- description: ''
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics NAV
provider_slug: navision
schema_file: json-schema/business-central-v2-journal-line-schema.json
slug: business-central-v2-journal-line
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JournalLine\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"journalId\": {\n      \"type\": \"string\"\n    },\n    \"journalDisplayName\": {\n      \"type\": \"string\"\n    },\n    \"lineNumber\": {\n      \"type\": \"integer\"\n    },\n    \"accountType\": {\n      \"type\": \"string\"\n    },\n    \"accountId\": {\n      \"type\": \"string\"\n    },\n    \"accountNumber\": {\n      \"type\": \"string\"\n    },\n    \"postingDate\": {\n      \"type\": \"string\"\n    },\n    \"documentNumber\": {\n      \"type\": \"string\"\n    },\n    \"externalDocumentNumber\": {\n      \"type\": \"string\"\n    },\n    \"amount\": {\n      \"type\": \"number\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"taxCode\": {\n      \"type\": \"string\"\n    },\n    \"\
  balanceAccountType\": {\n      \"type\": \"string\"\n    },\n    \"balanceAccountNumber\": {\n      \"type\": \"string\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/navision/refs/heads/main/json-schema/business-central-v2-journal-line-schema.json
tags:
- Business Management
- Dynamics NAV
- ERP
- Finance
- Inventory
- Microsoft
- Navision
title: JournalLine
---
