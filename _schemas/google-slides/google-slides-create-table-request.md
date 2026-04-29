---
description: Creates a new table.
layout: schema
name: CreateTableRequest
properties_list:
- description: A user-supplied object ID.
  name: objectId
  type: string
- description: Number of rows in the table.
  name: rows
  type: integer
- description: Number of columns in the table.
  name: columns
  type: integer
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-create-table-request-schema.json
slug: google-slides-create-table-request
source_filename: google-slides-create-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTableRequest\",\n  \"type\": \"object\",\n  \"description\": \"Creates a new table.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"A user-supplied object ID.\"\n    },\n    \"rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows in the table.\"\n    },\n    \"columns\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of columns in the table.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-create-table-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: CreateTableRequest
---
