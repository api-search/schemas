---
description: LiteralExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: LiteralExpression
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: term
  type: object
- description: ''
  name: value
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-literal-expression-schema.json
slug: rest-catalog-open-api-literal-expression
source_filename: rest-catalog-open-api-literal-expression-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-literal-expression-schema.json\",\n  \"title\": \"LiteralExpression\",\n  \"description\": \"LiteralExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"enum\": [\n        \"lt\",\n        \"lt-eq\",\n        \"gt\",\n        \"gt-eq\",\n        \"eq\",\n        \"not-eq\",\n        \"starts-with\",\n        \"not-starts-with\"\n      ]\n    },\n    \"term\": {\n      \"$ref\": \"#/components/schemas/Term\"\n    },\n    \"value\": {\n      \"$ref\": \"#/components/schemas/PrimitiveTypeValue\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"term\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-literal-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: LiteralExpression
---
