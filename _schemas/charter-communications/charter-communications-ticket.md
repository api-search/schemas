---
description: ''
layout: schema
name: Spectrum Enterprise Service Ticket
properties_list:
- description: ''
  name: ticketId
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: priority
  type: string
- description: ''
  name: accountId
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Charter Communications
provider_slug: charter-communications
schema_file: json-schema/charter-communications-ticket-schema.json
slug: charter-communications-ticket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://enterprise.spectrum.com/schemas/ticket.json\",\n  \"title\": \"Spectrum Enterprise Service Ticket\",\n  \"type\": \"object\",\n  \"required\": [\"ticketId\", \"subject\", \"status\"],\n  \"properties\": {\n    \"ticketId\": { \"type\": \"string\" },\n    \"subject\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"new\", \"open\", \"in-progress\", \"pending\", \"resolved\", \"closed\"]\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"enum\": [\"low\", \"normal\", \"high\", \"critical\"]\n    },\n    \"accountId\": { \"type\": \"string\" },\n    \"createdAt\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"updatedAt\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/charter-communications/refs/heads/main/json-schema/charter-communications-ticket-schema.json
tags:
- Broadband
- Cable
- CAMARA
- Enterprise
- Network as a Service
- NaaS
- Spectrum
- Telecommunications
- Ticketing
title: Spectrum Enterprise Service Ticket
---
