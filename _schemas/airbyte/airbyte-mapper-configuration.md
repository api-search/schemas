---
description: The values required to configure the mapper.
layout: schema
name: MapperConfiguration
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-mapper-configuration-schema.json
slug: airbyte-mapper-configuration
source_filename: airbyte-mapper-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-mapper-configuration-schema.json\",\n  \"title\": \"MapperConfiguration\",\n  \"description\": \"The values required to configure the mapper.\",\n  \"type\": \"object\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/HashingMapperConfiguration\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FieldFilteringMapperConfiguration\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FieldRenamingMapperConfiguration\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/RowFilteringMapperConfiguration\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/EncryptionMapperConfiguration\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: MapperConfiguration
---
