---
description: Writable fields for creating or updating a Look
layout: schema
name: WriteLookWithQuery
properties_list:
- description: Display title
  name: title
  type: string
- description: Description of the Look
  name: description
  type: string
- description: Space (folder) ID to place the Look in
  name: space_id
  type: string
- description: Folder ID to place the Look in
  name: folder_id
  type: string
- description: ID of the query to use
  name: query_id
  type: integer
- description: Whether the Look is public
  name: public
  type: boolean
- description: Whether to auto-run the query on load
  name: is_run_on_load
  type: boolean
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-write-look-with-query-schema.json
slug: looker-write-look-with-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WriteLookWithQuery\",\n  \"type\": \"object\",\n  \"description\": \"Writable fields for creating or updating a Look\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the Look\"\n    },\n    \"space_id\": {\n      \"type\": \"string\",\n      \"description\": \"Space (folder) ID to place the Look in\"\n    },\n    \"folder_id\": {\n      \"type\": \"string\",\n      \"description\": \"Folder ID to place the Look in\"\n    },\n    \"query_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the query to use\"\n    },\n    \"public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the Look is public\"\n    },\n    \"is_run_on_load\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ to auto-run the query on load\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-write-look-with-query-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: WriteLookWithQuery
---
