---
description: Provides details of a single permission.
layout: schema
name: PermissionResponse
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
  name: workspaceId
  type: object
- description: ''
  name: organizationId
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-permission-response-schema.json
slug: airbyte-permission-response
source_filename: airbyte-permission-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-response-schema.json\",\n  \"title\": \"PermissionResponse\",\n  \"description\": \"Provides details of a single permission.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/UserId\"\n    },\n    \"workspaceId\": {\n      \"$ref\": \"#/components/schemas/WorkspaceId\"\n    },\n    \"organizationId\": {\n      \"$ref\": \"#/components/schemas/OrganizationId\"\n    }\n  },\n  \"required\": [\n    \"permissionId\",\n    \"permissionType\",\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PermissionResponse
---
