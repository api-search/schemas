---
description: Properties and contents of each row in a table.
layout: schema
name: TableRow
properties_list:
- description: Properties and contents of each cell. Cells that span multiple columns are represented only once with a columnSpan greater than 1.
  name: tableCells
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-row-schema.json
slug: google-slides-table-row
source_filename: google-slides-table-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableRow\",\n  \"type\": \"object\",\n  \"description\": \"Properties and contents of each row in a table.\",\n  \"properties\": {\n    \"tableCells\": {\n      \"type\": \"array\",\n      \"description\": \"Properties and contents of each cell. Cells that span multiple columns are represented only once with a columnSpan greater than 1.\\n\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-row-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TableRow
---
