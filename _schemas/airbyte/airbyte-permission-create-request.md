---
description: PermissionCreateRequest schema from Airbyte API
layout: schema
name: PermissionCreateRequest
properties_list:
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
schema_file: json-schema/airbyte-permission-create-request-schema.json
slug: airbyte-permission-create-request
source_filename: airbyte-permission-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-create-request-schema.json\",\n  \"title\": \"PermissionCreateRequest\",\n  \"description\": \"PermissionCreateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PublicPermissionType\"\n    },\n    \"userId\": {\n      \"$ref\": \"#/components/schemas/UserId\"\n    },\n    \"workspaceId\": {\n      \"$ref\": \"#/components/schemas/WorkspaceId\"\n    },\n    \"organizationId\": {\n      \"$ref\": \"#/components/schemas/OrganizationId\"\n    }\n  },\n  \"required\": [\n    \"permissionType\",\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PermissionCreateRequest
---
