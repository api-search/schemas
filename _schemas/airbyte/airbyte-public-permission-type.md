---
description: Subset of `PermissionType` (removing `instance_admin`), could be used in public-api.
layout: schema
name: PublicPermissionType
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-public-permission-type-schema.json
slug: airbyte-public-permission-type
source_filename: airbyte-public-permission-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-public-permission-type-schema.json\",\n  \"title\": \"PublicPermissionType\",\n  \"description\": \"Subset of `PermissionType` (removing `instance_admin`), could be used in public-api.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"organization_admin\",\n    \"organization_editor\",\n    \"organization_runner\",\n    \"organization_reader\",\n    \"organization_member\",\n    \"workspace_admin\",\n    \"workspace_editor\",\n    \"workspace_runner\",\n    \"workspace_reader\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-public-permission-type-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: PublicPermissionType
---
