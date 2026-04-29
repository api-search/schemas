---
description: RemoveEncryptionKeyUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: RemoveEncryptionKeyUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: key-id
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remove-encryption-key-update-schema.json
slug: rest-catalog-open-api-remove-encryption-key-update
source_filename: rest-catalog-open-api-remove-encryption-key-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-encryption-key-update-schema.json\",\n  \"title\": \"RemoveEncryptionKeyUpdate\",\n  \"description\": \"RemoveEncryptionKeyUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"remove-encryption-key\"\n    },\n    \"key-id\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"key-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-encryption-key-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoveEncryptionKeyUpdate
---
