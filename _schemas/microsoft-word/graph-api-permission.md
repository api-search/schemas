---
description: Represents a sharing permission on a drive item.
layout: schema
name: Permission
properties_list:
- description: The unique identifier of the permission.
  name: id
  type: string
- description: The type of permission (read, write, owner).
  name: roles
  type: array
- description: ''
  name: link
  type: object
- description: ''
  name: grantedTo
  type: object
provider_name: Microsoft Word
provider_slug: microsoft-word
schema_file: json-schema/graph-api-permission-schema.json
slug: graph-api-permission
source_filename: graph-api-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/graph-api-permission-schema.json\",\n  \"title\": \"Permission\",\n  \"description\": \"Represents a sharing permission on a drive item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the permission.\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"The type of permission (read, write, owner).\"\n    },\n    \"link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"description\": \"The type of sharing link.\" },\n        \"webUrl\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"The URL of the sharing link.\" },\n        \"scope\": { \"type\": \"string\", \"description\"\
  : \"The scope of the link.\" }\n      }\n    },\n    \"grantedTo\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": { \"type\": \"string\" },\n            \"displayName\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-word/refs/heads/main/json-schema/graph-api-permission-schema.json
tags:
- Documents
- Microsoft 365
- Office
- Productivity
- Word Processing
title: Permission
---
