---
description: DataplaneCreateRequest schema from Airbyte API
layout: schema
name: DataplaneCreateRequest
properties_list:
- description: ''
  name: regionId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: enabled
  type: boolean
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-dataplane-create-request-schema.json
slug: airbyte-dataplane-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-dataplane-create-request-schema.json\",\n  \"title\": \"DataplaneCreateRequest\",\n  \"description\": \"DataplaneCreateRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"regionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"regionId\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-dataplane-create-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: DataplaneCreateRequest
---
