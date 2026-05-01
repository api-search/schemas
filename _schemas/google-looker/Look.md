---
description: A saved Looker Look (visualized query) that can be run, embedded, or rendered in a dashboard.
layout: schema
name: Look
properties_list:
- description: Unique identifier for the Look.
  name: id
  type: string
- description: Display title of the Look.
  name: title
  type: string
- description: Author-provided description of the Look.
  name: description
  type: string
- description: Indicates whether the Look is publicly accessible.
  name: public
  type: boolean
- description: Identifier of the underlying query used to render the Look.
  name: query_id
  type: string
- description: Identifier of the Looker user that owns the Look.
  name: user_id
  type: string
- description: Identifier of the folder where the Look is stored.
  name: folder_id
  type: string
provider_name: Google Looker
provider_slug: google-looker
schema_file: json-schema/Look.json
slug: Look
source_filename: Look.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/google-looker/json-schema/Look.json\",\n  \"title\": \"Look\",\n  \"description\": \"A saved Looker Look (visualized query) that can be run, embedded, or rendered in a dashboard.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the Look.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Display title of the Look.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Author-provided description of the Look.\"\n    },\n    \"public\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the Look is publicly accessible.\"\n    },\n    \"query_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the underlying query used to render the Look.\"\n    },\n    \"user_id\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Looker user that owns the Look.\"\n    },\n    \"folder_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the folder where the Look is stored.\"\n    }\n  },\n  \"required\": [\"id\", \"title\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/json-schema/Look.json
tags: []
title: Look
---
