---
description: EncryptionMapperConfiguration schema from Airbyte API
layout: schema
name: EncryptionMapperConfiguration
properties_list: []
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-encryption-mapper-configuration-schema.json
slug: airbyte-encryption-mapper-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-configuration-schema.json\",\n  \"title\": \"EncryptionMapperConfiguration\",\n  \"description\": \"EncryptionMapperConfiguration schema from Airbyte API\",\n  \"type\": \"object\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/EncryptionMapperRSAConfiguration\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/EncryptionMapperAESConfiguration\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-encryption-mapper-configuration-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: EncryptionMapperConfiguration
---
