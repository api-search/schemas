---
description: EncryptedKey schema from Apache Iceberg REST Catalog API
layout: schema
name: EncryptedKey
properties_list:
- description: ''
  name: key-id
  type: string
- description: ''
  name: encrypted-key-metadata
  type: string
- description: ''
  name: encrypted-by-id
  type: string
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-encrypted-key-schema.json
slug: rest-catalog-open-api-encrypted-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-encrypted-key-schema.json\",\n  \"title\": \"EncryptedKey\",\n  \"description\": \"EncryptedKey schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key-id\": {\n      \"type\": \"string\"\n    },\n    \"encrypted-key-metadata\": {\n      \"type\": \"string\",\n      \"format\": \"byte\",\n      \"contentEncoding\": \"base64\"\n    },\n    \"encrypted-by-id\": {\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"key-id\",\n    \"encrypted-key-metadata\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-encrypted-key-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: EncryptedKey
---
