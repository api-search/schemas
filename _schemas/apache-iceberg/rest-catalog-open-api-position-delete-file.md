---
description: PositionDeleteFile schema from Apache Iceberg REST Catalog API
layout: schema
name: PositionDeleteFile
properties_list:
- description: ''
  name: content
  type: string
- description: Offset within the delete file of delete content
  name: content-offset
  type: integer
- description: Length, in bytes, of the delete content; required if content-offset is present
  name: content-size-in-bytes
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-position-delete-file-schema.json
slug: rest-catalog-open-api-position-delete-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-position-delete-file-schema.json\",\n  \"title\": \"PositionDeleteFile\",\n  \"description\": \"PositionDeleteFile schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"const\": \"position-deletes\"\n    },\n    \"content-offset\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Offset within the delete file of delete content\"\n    },\n    \"content-size-in-bytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Length, in bytes, of the delete content; required if content-offset is present\"\n    }\n  },\n  \"required\": [\n    \"content\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/ContentFile\"\n    }\n\
  \  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-position-delete-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: PositionDeleteFile
---
