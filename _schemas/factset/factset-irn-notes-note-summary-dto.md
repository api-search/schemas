---
description: ''
layout: schema
name: NoteSummaryDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: date
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: authorId
  type: string
- description: ''
  name: contributorId
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: subjectId
  type: string
- description: ''
  name: isPersonal
  type: boolean
- description: ''
  name: state
  type: string
- description: ''
  name: approvalStatus
  type: string
- description: ''
  name: attachmentIds
  type: array
- description: ''
  name: relatedSymbols
  type: array
- description: ''
  name: recommendationId
  type: string
- description: ''
  name: sentimentId
  type: string
- description: ''
  name: customFields
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-notes-note-summary-dto-schema.json
slug: factset-irn-notes-note-summary-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NoteSummaryDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"authorId\": {\n      \"type\": \"string\"\n    },\n    \"contributorId\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"subjectId\": {\n      \"type\": \"string\"\n    },\n    \"isPersonal\": {\n      \"type\": \"boolean\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"approvalStatus\": {\n      \"type\": \"string\"\n    },\n    \"attachmentIds\": {\n      \"type\": \"array\"\n    },\n    \"relatedSymbols\": {\n      \"type\": \"array\"\n    },\n    \"recommendationId\": {\n      \"type\": \"string\"\n    },\n    \"sentimentId\": {\n\
  \      \"type\": \"string\"\n    },\n    \"customFields\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-notes-note-summary-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: NoteSummaryDto
---
