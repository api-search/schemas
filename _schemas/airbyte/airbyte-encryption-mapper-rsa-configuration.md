---
description: EncryptionMapperRSAConfiguration schema from Airbyte API
layout: schema
name: EncryptionMapperRSAConfiguration
properties_list:
- description: ''
  name: algorithm
  type: object
- description: ''
  name: fieldNameSuffix
  type: string
- description: ''
  name: publicKey
  type: string
- description: ''
  name: targetField
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-encryption-mapper-rsa-configuration-schema.json
slug: airbyte-encryption-mapper-rsa-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-rsa-configuration-schema.json\",\n  \"title\": \"EncryptionMapperRSAConfiguration\",\n  \"description\": \"EncryptionMapperRSAConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"algorithm\": {\n      \"$ref\": \"#/components/schemas/EncryptionMapperAlgorithm\"\n    },\n    \"fieldNameSuffix\": {\n      \"type\": \"string\"\n    },\n    \"publicKey\": {\n      \"type\": \"string\"\n    },\n    \"targetField\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"algorithm\",\n    \"publicKey\",\n    \"targetField\",\n    \"fieldNameSuffix\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-rsa-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EncryptionMapperRSAConfiguration
---
