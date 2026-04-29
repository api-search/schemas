---
description: A Snowflake view
layout: schema
name: View
properties_list:
- description: Name of the view
  name: name
  type: string
- description: Whether or not this view is secure
  name: secure
  type: boolean
- description: Kind of the view, permanent (default) or temporary
  name: kind
  type: string
- description: Whether or not this view can refer to itself using recursive syntax withot requiring a CTE (common table expression)
  name: recursive
  type: boolean
- description: The columns of the view
  name: columns
  type: array
- description: user comment associated to an object in the dictionary
  name: comment
  type: string
- description: Query used to create the view
  name: query
  type: string
- description: Date and time when the view was created.
  name: created_on
  type: string
- description: Database in which the view is stored
  name: database_name
  type: string
- description: Schema in which the view is stored
  name: schema_name
  type: string
- description: Role that owns the view
  name: owner
  type: string
- description: The type of role that owns the view
  name: owner_role_type
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/view-view-schema.json
slug: view-view
source_filename: view-view-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"View\",\n  \"type\": \"object\",\n  \"description\": \"A Snowflake view\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the view\"\n    },\n    \"secure\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not this view is secure\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Kind of the view, permanent (default) or temporary\"\n    },\n    \"recursive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether or not this view can refer to itself using recursive syntax withot requiring a CTE (common table expression)\"\n    },\n    \"columns\": {\n      \"type\": \"array\",\n      \"description\": \"The columns of the view\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"user comment associated to an object in the dictionary\"\n    },\n \
  \   \"query\": {\n      \"type\": \"string\",\n      \"description\": \"Query used to create the view\"\n    },\n    \"created_on\": {\n      \"type\": \"string\",\n      \"description\": \"Date and time when the view was created.\"\n    },\n    \"database_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database in which the view is stored\"\n    },\n    \"schema_name\": {\n      \"type\": \"string\",\n      \"description\": \"Schema in which the view is stored\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Role that owns the view\"\n    },\n    \"owner_role_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of role that owns the view\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/view-view-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: View
---
