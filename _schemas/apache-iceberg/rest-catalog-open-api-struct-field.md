---
description: StructField schema from Apache Iceberg REST Catalog API
layout: schema
name: StructField
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: object
- description: ''
  name: required
  type: boolean
- description: ''
  name: doc
  type: string
- description: ''
  name: initial-default
  type: object
- description: ''
  name: write-default
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-struct-field-schema.json
slug: rest-catalog-open-api-struct-field
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-struct-field-schema.json\",\n  \"title\": \"StructField\",\n  \"description\": \"StructField schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"$ref\": \"#/components/schemas/Type\"\n    },\n    \"required\": {\n      \"type\": \"boolean\"\n    },\n    \"doc\": {\n      \"type\": \"string\"\n    },\n    \"initial-default\": {\n      \"$ref\": \"#/components/schemas/PrimitiveTypeValue\"\n    },\n    \"write-default\": {\n      \"$ref\": \"#/components/schemas/PrimitiveTypeValue\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"type\",\n    \"required\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-struct-field-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: StructField
---
