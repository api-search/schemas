---
description: ConfiguredStreamMapper schema from Airbyte API
layout: schema
name: ConfiguredStreamMapper
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: object
- description: ''
  name: mapperConfiguration
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-configured-stream-mapper-schema.json
slug: airbyte-configured-stream-mapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-configured-stream-mapper-schema.json\",\n  \"title\": \"ConfiguredStreamMapper\",\n  \"description\": \"ConfiguredStreamMapper schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\"\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/StreamMapperType\"\n    },\n    \"mapperConfiguration\": {\n      \"$ref\": \"#/components/schemas/MapperConfiguration\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"mapperConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-configured-stream-mapper-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: ConfiguredStreamMapper
---
