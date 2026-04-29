---
description: HashingMapperConfiguration schema from Airbyte API
layout: schema
name: HashingMapperConfiguration
properties_list:
- description: The suffix to append to the field name after hashing.
  name: fieldNameSuffix
  type: string
- description: The hashing algorithm to use.
  name: method
  type: string
- description: The name of the field to be hashed.
  name: targetField
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-hashing-mapper-configuration-schema.json
slug: airbyte-hashing-mapper-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-hashing-mapper-configuration-schema.json\",\n  \"title\": \"HashingMapperConfiguration\",\n  \"description\": \"HashingMapperConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldNameSuffix\": {\n      \"type\": \"string\",\n      \"title\": \"Field name suffix\",\n      \"description\": \"The suffix to append to the field name after hashing.\"\n    },\n    \"method\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MD2\",\n        \"MD5\",\n        \"SHA-1\",\n        \"SHA-224\",\n        \"SHA-256\",\n        \"SHA-384\",\n        \"SHA-512\"\n      ],\n      \"title\": \"Hashing method\",\n      \"description\": \"The hashing algorithm to use.\"\n    },\n    \"targetField\": {\n      \"type\": \"string\",\n      \"title\": \"Original Field Name\"\
  ,\n      \"description\": \"The name of the field to be hashed.\"\n    }\n  },\n  \"required\": [\n    \"fieldNameSuffix\",\n    \"method\",\n    \"targetField\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-hashing-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: HashingMapperConfiguration
---
