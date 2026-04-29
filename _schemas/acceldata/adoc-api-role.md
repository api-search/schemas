---
description: A role with associated permissions
layout: schema
name: Role
properties_list:
- description: Role identifier
  name: id
  type: string
- description: Role name
  name: name
  type: string
- description: Role description
  name: description
  type: string
- description: List of permissions assigned to this role
  name: permissions
  type: array
provider_name: Acceldata
provider_slug: acceldata
schema_file: json-schema/adoc-api-role-schema.json
slug: adoc-api-role
source_filename: adoc-api-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://acceldata.io/schemas/role.json\",\n  \"title\": \"Role\",\n  \"type\": \"object\",\n  \"description\": \"A role with associated permissions\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Role identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Role name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Role description\"\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"List of permissions assigned to this role\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceldata/refs/heads/main/json-schema/adoc-api-role-schema.json
tags:
- AI Agents
- Data Management
- Data Observability
- Data Pipeline
- Data Quality
- Intelligence
- Observability
title: Role
---
