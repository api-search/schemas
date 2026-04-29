---
description: Describes what actions/endpoints the permission entitles to
layout: schema
name: PermissionType
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-permission-type-schema.json
slug: airbyte-permission-type
source_filename: airbyte-permission-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-type-schema.json\",\n  \"title\": \"PermissionType\",\n  \"description\": \"Describes what actions/endpoints the permission entitles to\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"instance_admin\",\n    \"organization_admin\",\n    \"organization_editor\",\n    \"organization_runner\",\n    \"organization_reader\",\n    \"organization_member\",\n    \"workspace_owner\",\n    \"workspace_admin\",\n    \"workspace_runner\",\n    \"workspace_editor\",\n    \"workspace_reader\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-permission-type-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PermissionType
---
