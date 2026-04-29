---
description: ContentFile schema from Apache Iceberg REST Catalog API
layout: schema
name: ContentFile
properties_list:
- description: ''
  name: content
  type: string
- description: ''
  name: file-path
  type: string
- description: ''
  name: file-format
  type: object
- description: ''
  name: spec-id
  type: integer
- description: A list of partition field values ordered based on the fields of the partition spec specified by the `spec-id`
  name: partition
  type: array
- description: Total file size in bytes
  name: file-size-in-bytes
  type: integer
- description: Number of records in the file
  name: record-count
  type: integer
- description: Encryption key metadata blob
  name: key-metadata
  type: object
- description: List of splittable offsets
  name: split-offsets
  type: array
- description: ''
  name: sort-order-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-content-file-schema.json
slug: rest-catalog-open-api-content-file
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-content-file-schema.json\",\n  \"title\": \"ContentFile\",\n  \"description\": \"ContentFile schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\"\n    },\n    \"file-path\": {\n      \"type\": \"string\"\n    },\n    \"file-format\": {\n      \"$ref\": \"#/components/schemas/FileFormat\"\n    },\n    \"spec-id\": {\n      \"type\": \"integer\"\n    },\n    \"partition\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PrimitiveTypeValue\"\n      },\n      \"description\": \"A list of partition field values ordered based on the fields of the partition spec specified by the `spec-id`\",\n      \"example\": [\n        1,\n        \"bar\"\n      ]\n    },\n\
  \    \"file-size-in-bytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total file size in bytes\"\n    },\n    \"record-count\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Number of records in the file\"\n    },\n    \"key-metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BinaryTypeValue\"\n        }\n      ],\n      \"description\": \"Encryption key metadata blob\"\n    },\n    \"split-offsets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"description\": \"List of splittable offsets\"\n    },\n    \"sort-order-id\": {\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"spec-id\",\n    \"partition\",\n    \"content\",\n    \"file-path\",\n    \"file-format\",\n    \"file-size-in-bytes\",\n    \"record-count\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-content-file-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ContentFile
---
