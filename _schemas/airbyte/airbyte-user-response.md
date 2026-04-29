---
description: Provides details of a single user in an organization.
layout: schema
name: UserResponse
properties_list:
- description: Name of the user
  name: name
  type: string
- description: ''
  name: id
  type: object
- description: ''
  name: email
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-user-response-schema.json
slug: airbyte-user-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-user-response-schema.json\",\n  \"title\": \"UserResponse\",\n  \"description\": \"Provides details of a single user in an organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of the user\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"$ref\": \"#/components/schemas/UserId\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"email\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-user-response-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: UserResponse
---
