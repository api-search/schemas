---
description: EmbeddedOrganizationListItem schema from Airbyte API
layout: schema
name: EmbeddedOrganizationListItem
properties_list:
- description: ''
  name: organizationId
  type: string
- description: ''
  name: organizationName
  type: string
- description: ''
  name: permission
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-embedded-organization-list-item-schema.json
slug: airbyte-embedded-organization-list-item
source_filename: airbyte-embedded-organization-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-organization-list-item-schema.json\",\n  \"title\": \"EmbeddedOrganizationListItem\",\n  \"description\": \"EmbeddedOrganizationListItem schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\"\n    },\n    \"permission\": {\n      \"$ref\": \"#/components/schemas/PermissionType\"\n    }\n  },\n  \"required\": [\n    \"organizationId\",\n    \"organizationName\",\n    \"permission\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-embedded-organization-list-item-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EmbeddedOrganizationListItem
---
