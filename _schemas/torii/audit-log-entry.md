---
description: An admin audit log entry recording an action performed within the Torii platform.
layout: schema
name: Torii Audit Log Entry
properties_list:
- description: Unique identifier for the audit log entry.
  name: id
  type: string
- description: The action that was performed.
  name: action
  type: string
- description: The user who performed the action.
  name: actor
  type: string
- description: Email of the user who performed the action.
  name: actorEmail
  type: string
- description: The target of the action.
  name: target
  type: string
- description: Additional details about the action.
  name: details
  type: object
- description: When the action was performed.
  name: createdAt
  type: string
provider_name: Torii
provider_slug: torii
schema_file: json-schema/audit-log-entry.json
slug: audit-log-entry
source_filename: audit-log-entry.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/audit-log-entry.json\",\n  \"title\": \"Torii Audit Log Entry\",\n  \"description\": \"An admin audit log entry recording an action performed within the Torii platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the audit log entry.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action that was performed.\"\n    },\n    \"actor\": {\n      \"type\": \"string\",\n      \"description\": \"The user who performed the action.\"\n    },\n    \"actorEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the user who performed the action.\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"The target of\
  \ the action.\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional details about the action.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the action was performed.\"\n    }\n  },\n  \"required\": [\"id\", \"action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/json-schema/audit-log-entry.json
tags:
- SaaS Management
title: Torii Audit Log Entry
---
