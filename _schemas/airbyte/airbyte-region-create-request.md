---
description: RegionCreateRequest schema from Airbyte API
layout: schema
name: RegionCreateRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: organizationId
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-region-create-request-schema.json
slug: airbyte-region-create-request
source_filename: airbyte-region-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-region-create-request-schema.json\",\n  \"title\": \"RegionCreateRequest\",\n  \"description\": \"RegionCreateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"organizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"organizationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-region-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: RegionCreateRequest
---
