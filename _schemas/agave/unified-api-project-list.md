---
description: Paginated list of projects.
layout: schema
name: ProjectList
properties_list:
- description: Array of project records.
  name: data
  type: array
- description: Cursor for the next page of results.
  name: next_cursor
  type: string
- description: Number of records returned.
  name: count
  type: integer
provider_name: Agave
provider_slug: agave
schema_file: json-schema/unified-api-project-list-schema.json
slug: unified-api-project-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-project-list-schema.json\",\n  \"title\": \"ProjectList\",\n  \"description\": \"Paginated list of projects.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of project records.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Project\"\n      },\n      \"example\": [\n        \"example_value\"\n      ]\n    },\n    \"next_cursor\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of results.\",\n      \"example\": \"eyJpZCI6MTIzfQ==\"\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records returned.\",\n      \"example\": 50\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agave/refs/heads/main/json-schema/unified-api-project-list-schema.json
tags:
- Accounting
- Construction
- Integration
title: ProjectList
---
