---
description: RowFilteringMapperConfiguration schema from Airbyte API
layout: schema
name: RowFilteringMapperConfiguration
properties_list:
- description: ''
  name: conditions
  type: object
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-row-filtering-mapper-configuration-schema.json
slug: airbyte-row-filtering-mapper-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-mapper-configuration-schema.json\",\n  \"title\": \"RowFilteringMapperConfiguration\",\n  \"description\": \"RowFilteringMapperConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"conditions\": {\n      \"$ref\": \"#/components/schemas/RowFilteringOperation\"\n    }\n  },\n  \"required\": [\n    \"conditions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-row-filtering-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: RowFilteringMapperConfiguration
---
