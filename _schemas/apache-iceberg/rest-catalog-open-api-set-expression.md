---
description: SetExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: SetExpression
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: term
  type: object
- description: ''
  name: values
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-expression-schema.json
slug: rest-catalog-open-api-set-expression
source_filename: rest-catalog-open-api-set-expression-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-expression-schema.json\",\n  \"title\": \"SetExpression\",\n  \"description\": \"SetExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"enum\": [\n        \"in\",\n        \"not-in\"\n      ]\n    },\n    \"term\": {\n      \"$ref\": \"#/components/schemas/Term\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PrimitiveTypeValue\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"term\",\n    \"values\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetExpression
---
