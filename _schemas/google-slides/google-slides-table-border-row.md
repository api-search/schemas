---
description: Contents of each border row in a table.
layout: schema
name: TableBorderRow
properties_list:
- description: Properties of each border cell.
  name: tableBorderCells
  type: array
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-border-row-schema.json
slug: google-slides-table-border-row
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableBorderRow\",\n  \"type\": \"object\",\n  \"description\": \"Contents of each border row in a table.\",\n  \"properties\": {\n    \"tableBorderCells\": {\n      \"type\": \"array\",\n      \"description\": \"Properties of each border cell.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-border-row-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TableBorderRow
---
