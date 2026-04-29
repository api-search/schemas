---
description: Reformat PermissionResponse with permission scope
layout: schema
name: PermissionResponseRead
properties_list:
- description: ''
  name: permissionId
  type: string
- description: ''
  name: permissionType
  type: object
- description: ''
  name: userId
  type: object
- description: ''
  name: scopeId
  type: string
- description: ''
  name: scope
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-permission-response-read-schema.json
slug: airbyte-permission-response-read
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-response-read-schema.json\",\n  \"title\": \"PermissionResponseRead\",\n  \"description\": \"Reformat PermissionResponse with permission scope\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/UserId\"\n    },\n    \"scopeId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"scope\": {\n      \"$ref\": \"#/components/schemas/PermissionScope\"\n    }\n  },\n  \"required\": [\n    \"permissionId\",\n    \"permissionType\",\n    \"userId\",\n    \"scope\",\n    \"scopeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-response-read-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PermissionResponseRead
---
