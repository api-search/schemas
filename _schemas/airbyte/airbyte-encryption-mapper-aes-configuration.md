---
description: EncryptionMapperAESConfiguration schema from Airbyte API
layout: schema
name: EncryptionMapperAESConfiguration
properties_list:
- description: ''
  name: algorithm
  type: object
- description: ''
  name: fieldNameSuffix
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: mode
  type: string
- description: ''
  name: padding
  type: string
- description: ''
  name: targetField
  type: string
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-encryption-mapper-aes-configuration-schema.json
slug: airbyte-encryption-mapper-aes-configuration
source_filename: airbyte-encryption-mapper-aes-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-aes-configuration-schema.json\",\n  \"title\": \"EncryptionMapperAESConfiguration\",\n  \"description\": \"EncryptionMapperAESConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"algorithm\": {\n      \"$ref\": \"#/components/schemas/EncryptionMapperAlgorithm\"\n    },\n    \"fieldNameSuffix\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"x-speakeasy-param-sensitive\": true\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CBC\",\n        \"CFB\",\n        \"OFB\",\n        \"CTR\",\n        \"GCM\",\n        \"ECB\"\n      ]\n    },\n    \"padding\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NoPadding\",\n        \"PKCS5Padding\"\n      ]\n    },\n\
  \    \"targetField\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"algorithm\",\n    \"key\",\n    \"mode\",\n    \"padding\",\n    \"targetField\",\n    \"fieldNameSuffix\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-aes-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EncryptionMapperAESConfiguration
---
