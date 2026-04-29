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
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-range-schema.json
slug: google-docs-v1-table-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableRange\",\n  \"type\": \"object\",\n  \"description\": \"A table range represents a reference to a subset of a table.\",\n  \"properties\": {\n    \"rowSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The row span of the table range.\"\n    },\n    \"columnSpan\": {\n      \"type\": \"integer\",\n      \"description\": \"The column span of the table range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-range-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableRange
---
