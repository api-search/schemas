---
description: Paginated list of users
layout: schema
name: UserList
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
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-user-list-schema.json
slug: adoc-api-user-list
source_filename: adoc-api-user-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/user-list.json\",\n  \"title\": \"UserList\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of users\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"user.json\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"page\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-user-list-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: UserList
---
