---
description: optional resource requirements to run workers (blank for unbounded allocations)
layout: schema
name: ResourceRequirements
properties_list:
- description: ''
  name: cpu_request
  type: string
- description: ''
  name: cpu_limit
  type: string
- description: ''
  name: memory_request
  type: string
- description: ''
  name: memory_limit
  type: string
- description: ''
  name: ephemeral_storage_request
  type: string
- description: ''
  name: ephemeral_storage_limit
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-resource-requirements-schema.json
slug: airbyte-resource-requirements
source_filename: airbyte-resource-requirements-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-resource-requirements-schema.json\",\n  \"title\": \"ResourceRequirements\",\n  \"description\": \"optional resource requirements to run workers (blank for unbounded allocations)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpu_request\": {\n      \"type\": \"string\"\n    },\n    \"cpu_limit\": {\n      \"type\": \"string\"\n    },\n    \"memory_request\": {\n      \"type\": \"string\"\n    },\n    \"memory_limit\": {\n      \"type\": \"string\"\n    },\n    \"ephemeral_storage_request\": {\n      \"type\": \"string\"\n    },\n    \"ephemeral_storage_limit\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-resource-requirements-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ResourceRequirements
---
