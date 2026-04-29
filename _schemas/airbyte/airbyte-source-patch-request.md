---
description: SourcePatchRequest schema from Airbyte API
layout: schema
name: SourcePatchRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: workspaceId
  type: string
- description: ''
  name: configuration
  type: object
- description: Optional secretID obtained through the OAuth redirect flow.
  name: secretId
  type: string
- description: ''
  name: resourceAllocation
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-source-patch-request-schema.json
slug: airbyte-source-patch-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-source-patch-request-schema.json\",\n  \"title\": \"SourcePatchRequest\",\n  \"description\": \"SourcePatchRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"My source\"\n    },\n    \"workspaceId\": {\n      \"format\": \"uuid\",\n      \"type\": \"string\"\n    },\n    \"configuration\": {\n      \"$ref\": \"#/components/schemas/SourceConfiguration\"\n    },\n    \"secretId\": {\n      \"description\": \"Optional secretID obtained through the  OAuth redirect flow.\",\n      \"type\": \"string\"\n    },\n    \"resourceAllocation\": {\n      \"$ref\": \"#/components/schemas/ScopedResourceRequirements\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-source-patch-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: SourcePatchRequest
---
