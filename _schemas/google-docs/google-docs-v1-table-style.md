---
description: Style properties for a table.
layout: schema
name: TableStyle
properties_list:
- description: The properties of each column.
  name: tableColumnProperties
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-table-style-schema.json
slug: google-docs-v1-table-style
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableStyle\",\n  \"type\": \"object\",\n  \"description\": \"Style properties for a table.\",\n  \"properties\": {\n    \"tableColumnProperties\": {\n      \"type\": \"array\",\n      \"description\": \"The properties of each column.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-table-style-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: TableStyle
---
