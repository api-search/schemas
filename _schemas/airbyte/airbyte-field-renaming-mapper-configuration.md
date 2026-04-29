---
description: FieldRenamingMapperConfiguration schema from Airbyte API
layout: schema
name: FieldRenamingMapperConfiguration
properties_list:
- description: The new name for the field after renaming.
  name: newFieldName
  type: string
- description: The current name of the field to rename.
  name: originalFieldName
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-field-renaming-mapper-configuration-schema.json
slug: airbyte-field-renaming-mapper-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-field-renaming-mapper-configuration-schema.json\",\n  \"title\": \"FieldRenamingMapperConfiguration\",\n  \"description\": \"FieldRenamingMapperConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"newFieldName\": {\n      \"type\": \"string\",\n      \"title\": \"New Field Name\",\n      \"description\": \"The new name for the field after renaming.\"\n    },\n    \"originalFieldName\": {\n      \"type\": \"string\",\n      \"title\": \"Original Field Name\",\n      \"description\": \"The current name of the field to rename.\"\n    }\n  },\n  \"required\": [\n    \"newFieldName\",\n    \"originalFieldName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-field-renaming-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: FieldRenamingMapperConfiguration
---
