---
description: ''
layout: schema
name: EventCreateRequest
properties_list:
- description: ''
  name: subject
  type: string
- description: ''
  name: locations
  type: array
- description: ''
  name: attendees
  type: array
- description: ''
  name: isAllDay
  type: boolean
- description: ''
  name: isOnlineMeeting
  type: boolean
- description: ''
  name: onlineMeetingProvider
  type: string
- description: ''
  name: showAs
  type: string
- description: ''
  name: importance
  type: string
- description: ''
  name: sensitivity
  type: string
- description: ''
  name: responseRequested
  type: boolean
- description: ''
  name: allowNewTimeProposals
  type: boolean
- description: ''
  name: categories
  type: array
- description: ''
  name: reminderMinutesBeforeStart
  type: integer
- description: ''
  name: transactionId
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-event-create-request-schema.json
slug: microsoft-graph-event-create-request
source_filename: microsoft-graph-event-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"locations\": {\n      \"type\": \"array\"\n    },\n    \"attendees\": {\n      \"type\": \"array\"\n    },\n    \"isAllDay\": {\n      \"type\": \"boolean\"\n    },\n    \"isOnlineMeeting\": {\n      \"type\": \"boolean\"\n    },\n    \"onlineMeetingProvider\": {\n      \"type\": \"string\"\n    },\n    \"showAs\": {\n      \"type\": \"string\"\n    },\n    \"importance\": {\n      \"type\": \"string\"\n    },\n    \"sensitivity\": {\n      \"type\": \"string\"\n    },\n    \"responseRequested\": {\n      \"type\": \"boolean\"\n    },\n    \"allowNewTimeProposals\": {\n      \"type\": \"boolean\"\n    },\n    \"categories\": {\n      \"type\": \"array\"\n    },\n    \"reminderMinutesBeforeStart\": {\n      \"type\": \"integer\"\n    },\n    \"transactionId\": {\n\
  \      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-event-create-request-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: EventCreateRequest
---
