---
description: ''
layout: schema
name: UpdateMeetingDto
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: identifier
  type: string
- description: ''
  name: start
  type: string
- description: ''
  name: end
  type: string
- description: ''
  name: locations
  type: array
- description: ''
  name: organizer
  type: string
- description: ''
  name: organizerId
  type: string
- description: ''
  name: attendees
  type: array
- description: ''
  name: alertAttendees
  type: boolean
- description: ''
  name: alertAuthor
  type: boolean
- description: ''
  name: relatedContacts
  type: array
- description: ''
  name: relatedSymbols
  type: array
- description: ''
  name: customFieldValues
  type: array
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-irn-meetings-update-meeting-dto-schema.json
slug: factset-irn-meetings-update-meeting-dto
source_filename: factset-irn-meetings-update-meeting-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateMeetingDto\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"identifier\": {\n      \"type\": \"string\"\n    },\n    \"start\": {\n      \"type\": \"string\"\n    },\n    \"end\": {\n      \"type\": \"string\"\n    },\n    \"locations\": {\n      \"type\": \"array\"\n    },\n    \"organizer\": {\n      \"type\": \"string\"\n    },\n    \"organizerId\": {\n      \"type\": \"string\"\n    },\n    \"attendees\": {\n      \"type\": \"array\"\n    },\n    \"alertAttendees\": {\n      \"type\": \"boolean\"\n    },\n    \"alertAuthor\": {\n      \"type\": \"boolean\"\n    },\n    \"relatedContacts\": {\n      \"type\": \"array\"\n    },\n    \"relatedSymbols\": {\n      \"type\": \"array\"\n    },\n    \"customFieldValues\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-irn-meetings-update-meeting-dto-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: UpdateMeetingDto
---
