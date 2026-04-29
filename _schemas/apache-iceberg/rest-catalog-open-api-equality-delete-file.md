---
description: EqualityDeleteFile schema from Apache Iceberg REST Catalog API
layout: schema
name: EqualityDeleteFile
properties_list:
- description: ''
  name: content
  type: string
- description: List of equality field IDs
  name: equality-ids
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-equality-delete-file-schema.json
slug: rest-catalog-open-api-equality-delete-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-equality-delete-file-schema.json\",\n  \"title\": \"EqualityDeleteFile\",\n  \"description\": \"EqualityDeleteFile schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"const\": \"equality-deletes\"\n    },\n    \"equality-ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"description\": \"List of equality field IDs\"\n    }\n  },\n  \"required\": [\n    \"content\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ContentFile\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-equality-delete-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: EqualityDeleteFile
---
