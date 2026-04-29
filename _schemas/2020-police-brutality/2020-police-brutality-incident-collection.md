---
description: Collection of police brutality incidents with metadata
layout: schema
name: IncidentCollection
properties_list:
- description: URL to the GitHub repository for editing/contributing
  name: edit_at
  type: string
- description: URL to report issues or get help
  name: help
  type: string
- description: Timestamp of the last data update
  name: updated_at
  type: string
- description: Array of incident records
  name: data
  type: array
provider_name: 2020 Police Brutality
provider_slug: 2020-police-brutality
schema_file: json-schema/2020-police-brutality-incident-collection-schema.json
slug: 2020-police-brutality-incident-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/2020-police-brutality/refs/heads/main/json-schema/2020-police-brutality-incident-collection-schema.json\",\n  \"title\": \"IncidentCollection\",\n  \"description\": \"Collection of police brutality incidents with metadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"edit_at\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the GitHub repository for editing/contributing\",\n      \"example\": \"https://github.com/2020PB/police-brutality\"\n    },\n    \"help\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to report issues or get help\",\n      \"example\": \"https://github.com/2020PB/police-brutality/issues\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last\
  \ data update\",\n      \"example\": \"2024-08-20T16:17:02Z\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of incident records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Incident\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/2020-police-brutality/refs/heads/main/json-schema/2020-police-brutality-incident-collection-schema.json
tags:
- Brutality
- Civil Rights
- Policing
- Public Data
title: IncidentCollection
---
