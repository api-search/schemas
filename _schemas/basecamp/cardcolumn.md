---
description: A column within a card table
layout: schema
name: CardColumn
properties_list:
- description: Column ID
  name: id
  type: integer
- description: Column title
  name: title
  type: string
- description: Column type (Kanban::Column, Kanban::Triage, etc.)
  name: type
  type: string
- description: Column color
  name: color
  type: string
- description: Column position within the table
  name: position
  type: integer
- description: Number of cards in this column
  name: cards_count
  type: integer
- description: API URL to list cards in this column
  name: cards_url
  type: string
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/cardcolumn-schema.json
slug: cardcolumn
source_filename: cardcolumn-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/cardcolumn-schema.json\",\n  \"title\": \"CardColumn\",\n  \"type\": \"object\",\n  \"description\": \"A column within a card table\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Column ID\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Column title\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Column type (Kanban::Column, Kanban::Triage, etc.)\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Column color\",\n      \"nullable\": true\n    },\n    \"position\": {\n      \"type\": \"integer\",\n      \"description\": \"Column position within the table\"\n    },\n    \"cards_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cards in this column\"\n    },\n    \"cards_url\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL to list cards in this column\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/cardcolumn-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: CardColumn
---
