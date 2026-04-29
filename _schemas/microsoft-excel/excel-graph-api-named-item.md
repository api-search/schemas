---
description: Represents a defined name for a cell range or value.
layout: schema
name: NamedItem
properties_list:
- description: The name of the named item.
  name: name
  type: string
- description: The type of the named item.
  name: type
  type: string
- description: The formula or range reference.
  name: value
  type: string
- description: Whether the named item is visible.
  name: visible
  type: boolean
provider_name: Microsoft Excel
provider_slug: microsoft-excel
schema_file: json-schema/excel-graph-api-named-item-schema.json
slug: excel-graph-api-named-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-named-item-schema.json\",\n  \"title\": \"NamedItem\",\n  \"description\": \"Represents a defined name for a cell range or value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the named item.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the named item.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The formula or range reference.\"\n    },\n    \"visible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the named item is visible.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-excel/refs/heads/main/json-schema/excel-graph-api-named-item-schema.json
tags:
- Automation
- Data Analysis
- Microsoft
- Microsoft 365
- Office
- Spreadsheets
title: NamedItem
---
