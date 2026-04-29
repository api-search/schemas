---
description: Represents a table in a Word document.
layout: schema
name: Table
properties_list:
- description: Unique identifier of the table.
  name: id
  type: string
- description: Number of rows in the table.
  name: rowCount
  type: integer
- description: Number of columns in the table.
  name: columnCount
  type: integer
- description: Style name applied to the table.
  name: style
  type: string
- description: Table alignment.
  name: alignment
  type: string
- description: Number of header rows.
  name: headerRowCount
  type: integer
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/javascript-api-table-schema.json
slug: javascript-api-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-table-schema.json\",\n  \"title\": \"Table\",\n  \"description\": \"Represents a table in a Word document.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the table.\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table.\"\n    },\n    \"columnCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns in the table.\"\n    },\n    \"style\": {\n      \"type\": \"string\",\n      \"description\": \"Style name applied to the table.\"\n    },\n    \"alignment\": {\n      \"type\": \"string\",\n      \"description\": \"Table alignment.\",\n      \"enum\": [\"Left\", \"Centered\", \"Right\"]\n    },\n    \"headerRowCount\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of header rows.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/javascript-api-table-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: Table
---
