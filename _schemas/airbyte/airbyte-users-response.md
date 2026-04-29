---
description: List/Array of multiple users in an organization
layout: schema
name: UsersResponse
properties_list:
- description: ''
  name: data
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-users-response-schema.json
slug: airbyte-users-response
source_filename: airbyte-users-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-users-response-schema.json\",\n  \"title\": \"UsersResponse\",\n  \"description\": \"List/Array of multiple users in an organization\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/UserResponse\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-users-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: UsersResponse
---
