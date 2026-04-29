---
description: ApplicationRead schema from Airbyte API
layout: schema
name: ApplicationRead
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: clientId
  type: string
- description: ''
  name: clientSecret
  type: string
- description: ''
  name: createdAt
  type: integer
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-application-read-schema.json
slug: airbyte-application-read
source_filename: airbyte-application-read-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-read-schema.json\",\n  \"title\": \"ApplicationRead\",\n  \"description\": \"ApplicationRead schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"clientId\": {\n      \"type\": \"string\"\n    },\n    \"clientSecret\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"clientId\",\n    \"clientSecret\",\n    \"createdAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-application-read-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ApplicationRead
---
