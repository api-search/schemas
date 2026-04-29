---
description: Provides details of a single group permission
layout: schema
name: GroupPermissionResponse
properties_list:
- description: The ID of the permission
  name: permissionId
  type: string
- description: The ID of the group
  name: groupId
  type: string
- description: ''
  name: permissionType
  type: object
- description: The workspace ID for workspace-scoped permissions
  name: workspaceId
  type: string
- description: The organization ID for organization-scoped permissions
  name: organizationId
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-permission-response-schema.json
slug: airbyte-group-permission-response
source_filename: airbyte-group-permission-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permission-response-schema.json\",\n  \"title\": \"GroupPermissionResponse\",\n  \"description\": \"Provides details of a single group permission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the permission\"\n    },\n    \"groupId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The ID of the group\"\n    },\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"The workspace ID for workspace-scoped permissions\"\n    },\n    \"organizationId\": {\n      \"type\": \"\
  string\",\n      \"format\": \"uuid\",\n      \"nullable\": true,\n      \"description\": \"The organization ID for organization-scoped permissions\"\n    }\n  },\n  \"required\": [\n    \"permissionId\",\n    \"groupId\",\n    \"permissionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permission-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupPermissionResponse
---
