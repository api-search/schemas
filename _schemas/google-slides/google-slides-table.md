---
description: A PageElement kind representing a table.
layout: schema
name: Table
properties_list:
- description: Number of rows in the table.
  name: rows
  type: integer
- description: Number of columns in the table.
  name: columns
  type: integer
- description: Properties and contents of each row. Cells that span multiple rows are contained in only one of these rows and have a rowSpan greater than 1.
  name: tableRows
  type: array
- description: Properties of each column.
  name: tableColumns
  type: array
- description: Properties of horizontal cell borders.
  name: horizontalBorderRows
  type: array
- description: Properties of vertical cell borders.
  name: verticalBorderRows
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-schema.json
slug: google-slides-table
source_filename: google-slides-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"description\": \"A PageElement kind representing a table.\\n\",\n  \"properties\": {\n    \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table.\"\n    },\n    \"columns\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns in the table.\"\n    },\n    \"tableRows\": {\n      \"type\": \"array\",\n      \"description\": \"Properties and contents of each row. Cells that span multiple rows are contained in only one of these rows and have a rowSpan greater than 1.\\n\"\n    },\n    \"tableColumns\": {\n      \"type\": \"array\",\n      \"description\": \"Properties of each column.\"\n    },\n    \"horizontalBorderRows\": {\n      \"type\": \"array\",\n      \"description\": \"Properties of horizontal cell borders.\"\n    },\n    \"verticalBorderRows\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Properties of vertical cell borders.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: Table
---
