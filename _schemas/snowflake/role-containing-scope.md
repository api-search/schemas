---
description: ''
layout: schema
name: ContainingScope
properties_list:
- description: Database name of the securable scope if applicable.
  name: database
  type: string
- description: Schema name of the securable scope if applicable.
  name: schema
  type: string
provider_name: Snowflake
provider_slug: snowflake
schema_file: json-schema/role-containing-scope-schema.json
slug: role-containing-scope
source_filename: role-containing-scope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainingScope\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"database\": {\n      \"type\": \"string\",\n      \"description\": \"Database name of the securable scope if applicable.\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Schema name of the securable scope if applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/snowflake/refs/heads/main/json-schema/role-containing-scope-schema.json
tags:
- Data Lakes
- Data Sharing
- Data Warehousing
- Database
- SQL
title: ContainingScope
---
