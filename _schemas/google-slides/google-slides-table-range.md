---
description: A table range represents a reference to a subset of a table.
layout: schema
name: TableRange
properties_list:
- description: The row span of the table range.
  name: rowSpan
  type: integer
- description: The column span of the table range.
  name: columnSpan
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-table-range-schema.json
slug: google-slides-table-range
source_filename: google-slides-table-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableRange\",\n  \"type\": \"object\",\n  \"description\": \"A table range represents a reference to a subset of a table.\",\n  \"properties\": {\n    \"rowSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The row span of the table range.\"\n    },\n    \"columnSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The column span of the table range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-table-range-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: TableRange
---
