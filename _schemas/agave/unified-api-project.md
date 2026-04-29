---
description: A construction project record from the linked source system.
layout: schema
name: Project
properties_list:
- description: Agave unified project identifier.
  name: id
  type: string
- description: Project identifier in the source system.
  name: source_id
  type: string
- description: Project name.
  name: name
  type: string
- description: Project number or code.
  name: number
  type: string
- description: Project status.
  name: status
  type: string
- description: Project address.
  name: address
  type: string
- description: Project start date.
  name: start_date
  type: string
- description: Estimated project completion date.
  name: estimated_completion_date
  type: string
- description: Total approved project budget in USD.
  name: total_budget
  type: number
- description: Timestamp when the record was created.
  name: created_at
  type: string
- description: Timestamp when the record was last updated.
  name: updated_at
  type: string
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-project-schema.json
slug: unified-api-project
source_filename: unified-api-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"A construction project record from the linked source system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Agave unified project identifier.\",\n      \"example\": \"proj-500123\"\n    },\n    \"source_id\": {\n      \"type\": \"string\",\n      \"description\": \"Project identifier in the source system.\",\n      \"example\": 12345\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Project name.\",\n      \"example\": \"Downtown Office Building\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Project number or code.\",\n      \"example\": \"2025-001\"\n    },\n    \"status\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Project status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"completed\"\n      ],\n      \"example\": \"active\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Project address.\",\n      \"example\": \"123 Main St, San Francisco, CA 94105\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Project start date.\",\n      \"example\": \"2025-01-15\"\n    },\n    \"estimated_completion_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Estimated project completion date.\",\n      \"example\": \"2026-06-30\"\n    },\n    \"total_budget\": {\n      \"type\": \"number\",\n      \"description\": \"Total approved project budget in USD.\",\n      \"example\": 5000000.0\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Timestamp when the record was created.\",\n      \"example\": \"2025-01-15T09:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last updated.\",\n      \"example\": \"2025-04-01T12:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-project-schema.json
tags:
- Accounting
- Construction
- Integration
title: Project
---
