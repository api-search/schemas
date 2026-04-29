---
description: StructType schema from Apache Iceberg REST Catalog API
layout: schema
name: StructType
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: fields
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-struct-type-schema.json
slug: rest-catalog-open-api-struct-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-struct-type-schema.json\",\n  \"title\": \"StructType\",\n  \"description\": \"StructType schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"struct\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StructField\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-struct-type-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: StructType
---
