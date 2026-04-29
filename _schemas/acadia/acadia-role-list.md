---
description: Paginated list of roles
layout: schema
name: RoleList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: page
  type: integer
- description: ''
  name: limit
  type: integer
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-role-list-schema.json
slug: acadia-role-list
source_filename: acadia-role-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-role-list-schema.json\",\n  \"title\": \"RoleList\",\n  \"description\": \"Paginated list of roles\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Role\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 8\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-role-list-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: RoleList
---
