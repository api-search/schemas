---
description: ListType schema from Apache Iceberg REST Catalog API
layout: schema
name: ListType
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: element-id
  type: integer
- description: ''
  name: element
  type: object
- description: ''
  name: element-required
  type: boolean
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-list-type-schema.json
slug: rest-catalog-open-api-list-type
source_filename: rest-catalog-open-api-list-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-list-type-schema.json\",\n  \"title\": \"ListType\",\n  \"description\": \"ListType schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"list\"\n    },\n    \"element-id\": {\n      \"type\": \"integer\"\n    },\n    \"element\": {\n      \"$ref\": \"#/components/schemas/Type\"\n    },\n    \"element-required\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"element-id\",\n    \"element\",\n    \"element-required\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-list-type-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ListType
---
