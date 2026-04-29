---
description: Updates the properties of a Table column.
layout: schema
name: UpdateTableColumnPropertiesRequest
properties_list:
- description: The object ID of the table.
  name: objectId
  type: string
- description: The list of zero-based indices specifying which columns to update.
  name: columnIndices
  type: array
- description: The fields that should be updated.
  name: fields
  type: string
provider_name: Google Slides
provider_slug: google-slides
schema_file: json-schema/google-slides-update-table-column-properties-request-schema.json
slug: google-slides-update-table-column-properties-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateTableColumnPropertiesRequest\",\n  \"type\": \"object\",\n  \"description\": \"Updates the properties of a Table column.\",\n  \"properties\": {\n    \"objectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object ID of the table.\"\n    },\n    \"columnIndices\": {\n      \"type\": \"array\",\n      \"description\": \"The list of zero-based indices specifying which columns to update.\"\n    },\n    \"fields\": {\n      \"type\": \"string\",\n      \"description\": \"The fields that should be updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-slides/refs/heads/main/json-schema/google-slides-update-table-column-properties-request-schema.json
tags:
- Collaboration
- Google Workspace
- Presentations
- Productivity
- Slides
title: UpdateTableColumnPropertiesRequest
---
