---
description: An Airtable view provides a filtered, sorted, and formatted perspective on the records in a table. Views control which fields are visible, how records are ordered, and which records meet the view's filter criteria.
layout: schema
name: Airtable View
properties_list:
- description: The unique identifier for the view. View IDs always start with the 'viw' prefix.
  name: id
  type: string
- description: The display name of the view.
  name: name
  type: string
- description: The type of view, which determines the layout and interaction model.
  name: type
  type: string
- description: If set, this is a personal view visible only to the specified user. Null indicates a shared view.
  name: personalForUserId
  type:
  - string
  - 'null'
- description: The IDs of fields visible in this view, in display order. Only included when explicitly requested via the include parameter.
  name: visibleFieldIds
  type: array
provider_name: Airtable
provider_slug: airtable
schema_file: json-schema/airtable-view-schema.json
slug: airtable-view
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.airtable.com/view.json\",\n  \"title\": \"Airtable View\",\n  \"description\": \"An Airtable view provides a filtered, sorted, and formatted perspective on the records in a table. Views control which fields are visible, how records are ordered, and which records meet the view's filter criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the view. View IDs always start with the 'viw' prefix.\",\n      \"pattern\": \"^viw[a-zA-Z0-9]+$\",\n      \"examples\": [\"viwABC123def456\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the view.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of view, which determines the layout and interaction model.\",\n      \"enum\": [\n        \"grid\",\n \
  \       \"form\",\n        \"calendar\",\n        \"gallery\",\n        \"kanban\",\n        \"timeline\",\n        \"block\"\n      ]\n    },\n    \"personalForUserId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If set, this is a personal view visible only to the specified user. Null indicates a shared view.\"\n    },\n    \"visibleFieldIds\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of fields visible in this view, in display order. Only included when explicitly requested via the include parameter.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^fld[a-zA-Z0-9]+$\"\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/json-schema/airtable-view-schema.json
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
title: Airtable View
---
