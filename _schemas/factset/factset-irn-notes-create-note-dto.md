---
description: ''
layout: schema
name: CreateNoteDto
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: date
  type: string
- description: ''
  name: subjectId
  type: string
- description: ''
  name: recommendationId
  type: string
- description: ''
  name: sentimentId
  type: string
- description: ''
  name: source
  type: string
- description: ''
  name: link
  type: string
- description: ''
  name: relatedSymbols
  type: array
- description: ''
  name: relatedContacts
  type: array
- description: ''
  name: customFieldValues
  type: array
- description: ''
  name: isPersonal
  type: boolean
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-notes-create-note-dto-schema.json
slug: factset-irn-notes-create-note-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateNoteDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"type\": \"string\"\n    },\n    \"subjectId\": {\n      \"type\": \"string\"\n    },\n    \"recommendationId\": {\n      \"type\": \"string\"\n    },\n    \"sentimentId\": {\n      \"type\": \"string\"\n    },\n    \"source\": {\n      \"type\": \"string\"\n    },\n    \"link\": {\n      \"type\": \"string\"\n    },\n    \"relatedSymbols\": {\n      \"type\": \"array\"\n    },\n    \"relatedContacts\": {\n      \"type\": \"array\"\n    },\n    \"customFieldValues\": {\n      \"type\": \"array\"\n    },\n    \"isPersonal\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-notes-create-note-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: CreateNoteDto
---
