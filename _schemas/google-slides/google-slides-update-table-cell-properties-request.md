---
description: Update the properties of a TableCell.
layout: schema
name: UpdateTableCellPropertiesRequest
properties_list:
- description: The object ID of the table.
  name: objectId
  type: string
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-table-cell-properties-request-schema.json
slug: google-slides-update-table-cell-properties-request
source_filename: google-slides-update-table-cell-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableCellPropertiesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Update the properties of a TableCell.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the table.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-table-cell-properties-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateTableCellPropertiesRequest
---
