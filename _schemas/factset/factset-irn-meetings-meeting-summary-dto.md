---
description: ''
layout: schema
name: MeetingSummaryDto
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: start
  type: string
- description: ''
  name: end
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: authorId
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: organizer
  type: string
- description: ''
  name: organizerId
  type: string
- description: ''
  name: attachmentIds
  type: array
- description: ''
  name: relatedSymbols
  type: array
- description: ''
  name: locations
  type: array
- description: ''
  name: attendees
  type: array
- description: ''
  name: customFieldValues
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-meetings-meeting-summary-dto-schema.json
slug: factset-irn-meetings-meeting-summary-dto
source_filename: factset-irn-meetings-meeting-summary-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingSummaryDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"start\": {\n      \"type\": \"string\"\n    },\n    \"end\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"authorId\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"organizer\": {\n      \"type\": \"string\"\n    },\n    \"organizerId\": {\n      \"type\": \"string\"\n    },\n    \"attachmentIds\": {\n      \"type\": \"array\"\n    },\n    \"relatedSymbols\": {\n      \"type\": \"array\"\n    },\n    \"locations\": {\n      \"type\": \"array\"\n    },\n    \"attendees\": {\n      \"type\": \"array\"\n    },\n    \"customFieldValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-meetings-meeting-summary-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: MeetingSummaryDto
---
