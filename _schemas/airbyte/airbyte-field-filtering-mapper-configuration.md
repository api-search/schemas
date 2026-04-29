---
description: FieldFilteringMapperConfiguration schema from Airbyte API
layout: schema
name: FieldFilteringMapperConfiguration
properties_list:
- description: The name of the field to filter.
  name: targetField
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-field-filtering-mapper-configuration-schema.json
slug: airbyte-field-filtering-mapper-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-field-filtering-mapper-configuration-schema.json\",\n  \"title\": \"FieldFilteringMapperConfiguration\",\n  \"description\": \"FieldFilteringMapperConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetField\": {\n      \"type\": \"string\",\n      \"title\": \"The Field to Filter\",\n      \"description\": \"The name of the field to filter.\"\n    }\n  },\n  \"required\": [\n    \"targetField\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-field-filtering-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: FieldFilteringMapperConfiguration
---
