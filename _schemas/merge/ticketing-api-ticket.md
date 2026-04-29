---
description: A ticket or issue from a connected ticketing or project management system.
layout: schema
name: Ticket
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: remote_id
  type: string
- description: Ticket title or name.
  name: name
  type: string
- description: ''
  name: assignees
  type: array
- description: ''
  name: creator
  type: string
- description: ''
  name: due_date
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: priority
  type: string
- description: ''
  name: ticket_type
  type: string
- description: ''
  name: account
  type: string
- description: ''
  name: contact
  type: string
- description: ''
  name: parent_ticket
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: completed_at
  type: string
- description: ''
  name: ticket_url
  type: string
- description: ''
  name: remote_was_deleted
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: modified_at
  type: string
provider_name: Merge
provider_slug: merge
schema_file: json-schema/ticketing-api-ticket-schema.json
slug: ticketing-api-ticket
source_filename: ticketing-api-ticket-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ticketing-api-ticket-schema.json\",\n  \"title\": \"Ticket\",\n  \"description\": \"A ticket or issue from a connected ticketing or project management system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Ticket title or name.\" },\n    \"assignees\": { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uuid\" } },\n    \"creator\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"due_date\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"OPEN\", \"CLOSED\", \"IN_PROGRESS\", \"ON_HOLD\"] },\n    \"description\": { \"type\": \"string\" },\n    \"priority\": { \"type\"\
  : \"string\", \"enum\": [\"URGENT\", \"HIGH\", \"NORMAL\", \"LOW\"] },\n    \"ticket_type\": { \"type\": \"string\" },\n    \"account\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"contact\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"parent_ticket\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"tags\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n    \"completed_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"ticket_url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"remote_was_deleted\": { \"type\": \"boolean\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modified_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ticketing-api-ticket-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Ticket
---
