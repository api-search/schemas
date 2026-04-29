---
description: AddEncryptionKeyUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: AddEncryptionKeyUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: encryption-key
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-add-encryption-key-update-schema.json
slug: rest-catalog-open-api-add-encryption-key-update
source_filename: rest-catalog-open-api-add-encryption-key-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-encryption-key-update-schema.json\",\n  \"title\": \"AddEncryptionKeyUpdate\",\n  \"description\": \"AddEncryptionKeyUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"add-encryption-key\"\n    },\n    \"encryption-key\": {\n      \"$ref\": \"#/components/schemas/EncryptedKey\"\n    }\n  },\n  \"required\": [\n    \"encryption-key\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-add-encryption-key-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AddEncryptionKeyUpdate
---
