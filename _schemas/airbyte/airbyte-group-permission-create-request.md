---
description: Request body for creating a group permission
layout: schema
name: GroupPermissionCreateRequest
properties_list:
- description: ''
  name: permissionType
  type: object
- description: Required for workspace-scoped permissions
  name: workspaceId
  type: string
- description: Required for organization-scoped permissions
  name: organizationId
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-permission-create-request-schema.json
slug: airbyte-group-permission-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permission-create-request-schema.json\",\n  \"title\": \"GroupPermissionCreateRequest\",\n  \"description\": \"Request body for creating a group permission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"Required for workspace-scoped permissions\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"Required for organization-scoped permissions\"\n    }\n  },\n  \"required\": [\n    \"permissionType\"\n  ],\n  \"oneOf\": [\n    {\n      \"required\": [\n        \"workspaceId\"\n   \
  \   ]\n    },\n    {\n      \"required\": [\n        \"organizationId\"\n      ]\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permission-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupPermissionCreateRequest
---
