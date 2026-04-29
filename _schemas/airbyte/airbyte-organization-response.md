---
description: Provides details of a single organization for a user.
layout: schema
name: OrganizationResponse
properties_list:
- description: ''
  name: organizationId
  type: object
- description: ''
  name: organizationName
  type: string
- description: ''
  name: email
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-organization-response-schema.json
slug: airbyte-organization-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-organization-response-schema.json\",\n  \"title\": \"OrganizationResponse\",\n  \"description\": \"Provides details of a single organization for a user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"organizationId\": {\n      \"$ref\": \"#/components/schemas/OrganizationId\"\n    },\n    \"organizationName\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    }\n  },\n  \"required\": [\n    \"organizationId\",\n    \"organizationName\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-organization-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: OrganizationResponse
---
