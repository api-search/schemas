---
description: Properties and contents of each table cell.
layout: schema
name: TableCell
properties_list:
- description: Row span of the cell.
  name: rowSpan
  type: integer
- description: Column span of the cell.
  name: columnSpan
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-cell-schema.json
slug: google-slides-table-cell
source_filename: google-slides-table-cell-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableCell\",\n  \"type\": \"object\",\n  \"description\": \"Properties and contents of each table cell.\",\n  \"properties\": {\n    \"rowSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"Row span of the cell.\"\n    },\n    \"columnSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"Column span of the cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-cell-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TableCell
---
