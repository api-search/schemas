---
description: TransformTerm schema from Apache Iceberg REST Catalog API
layout: schema
name: TransformTerm
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: transform
  type: object
- description: ''
  name: term
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-transform-term-schema.json
slug: rest-catalog-open-api-transform-term
source_filename: rest-catalog-open-api-transform-term-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-transform-term-schema.json\",\n  \"title\": \"TransformTerm\",\n  \"description\": \"TransformTerm schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"transform\"\n    },\n    \"transform\": {\n      \"$ref\": \"#/components/schemas/Transform\"\n    },\n    \"term\": {\n      \"$ref\": \"#/components/schemas/Reference\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"transform\",\n    \"term\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-transform-term-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TransformTerm
---
