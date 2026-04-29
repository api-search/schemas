---
description: List/Array of group permissions
layout: schema
name: GroupPermissionsResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-group-permissions-response-schema.json
slug: airbyte-group-permissions-response
source_filename: airbyte-group-permissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permissions-response-schema.json\",\n  \"title\": \"GroupPermissionsResponse\",\n  \"description\": \"List/Array of group permissions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/GroupPermissionResponse\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-group-permissions-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: GroupPermissionsResponse
---
