---
description: A sales opportunity or deal from a connected CRM system.
layout: schema
name: Opportunity
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: remote_id
  type: string
- description: Opportunity name.
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Deal value in cents.
  name: amount
  type: integer
- description: ''
  name: owner
  type: string
- description: ''
  name: account
  type: string
- description: ''
  name: stage
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: close_date
  type: string
- description: ''
  name: last_activity_at
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
schema_file: json-schema/crm-api-opportunity-schema.json
slug: crm-api-opportunity
source_filename: crm-api-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/crm-api-opportunity-schema.json\",\n  \"title\": \"Opportunity\",\n  \"description\": \"A sales opportunity or deal from a connected CRM system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"remote_id\": { \"type\": \"string\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Opportunity name.\" },\n    \"description\": { \"type\": \"string\" },\n    \"amount\": { \"type\": \"integer\", \"description\": \"Deal value in cents.\" },\n    \"owner\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"account\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"stage\": { \"type\": \"string\", \"format\": \"uuid\" },\n    \"status\": { \"type\": \"string\", \"enum\": [\"OPEN\", \"WON\", \"LOST\"] },\n    \"close_date\": { \"type\"\
  : \"string\", \"format\": \"date-time\" },\n    \"last_activity_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"remote_was_deleted\": { \"type\": \"boolean\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modified_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/crm-api-opportunity-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Opportunity
---
