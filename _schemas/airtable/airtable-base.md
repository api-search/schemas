---
description: An Airtable base is a database that contains one or more tables. Bases are the top-level containers for organizing related data in Airtable.
layout: schema
name: Airtable Base
properties_list:
- description: The unique identifier for the base. Base IDs always start with the 'app' prefix.
  name: id
  type: string
- description: The display name of the base.
  name: name
  type: string
- description: The permission level the authenticated user has on this base.
  name: permissionLevel
  type: string
- description: The tables contained within this base. Only included when retrieving the full base schema.
  name: tables
  type: array
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-base-schema.json
slug: airtable-base
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/base.json\",\n  \"title\": \"Airtable Base\",\n  \"description\": \"An Airtable base is a database that contains one or more tables. Bases are the top-level containers for organizing related data in Airtable.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the base. Base IDs always start with the 'app' prefix.\",\n      \"pattern\": \"^app[a-zA-Z0-9]+$\",\n      \"examples\": [\"appABC123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the base.\"\n    },\n    \"permissionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The permission level the authenticated user has on this base.\",\n      \"enum\": [\"none\", \"read\", \"comment\", \"edit\", \"create\"]\n    },\n    \"tables\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"The tables contained within this base. Only included when retrieving the full base schema.\",\n      \"items\": {\n        \"$ref\": \"https://schemas.airtable.com/table.json\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-base-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable Base
---
