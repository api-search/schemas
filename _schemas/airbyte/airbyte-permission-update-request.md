---
description: PermissionUpdateRequest schema from Airbyte API
layout: schema
name: PermissionUpdateRequest
properties_list:
- description: ''
  name: permissionType
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-permission-update-request-schema.json
slug: airbyte-permission-update-request
source_filename: airbyte-permission-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-update-request-schema.json\",\n  \"title\": \"PermissionUpdateRequest\",\n  \"description\": \"PermissionUpdateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permissionType\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    }\n  },\n  \"required\": [\n    \"permissionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-update-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PermissionUpdateRequest
---
