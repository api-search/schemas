---
description: UnaryExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: UnaryExpression
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: term
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-unary-expression-schema.json
slug: rest-catalog-open-api-unary-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-unary-expression-schema.json\",\n  \"title\": \"UnaryExpression\",\n  \"description\": \"UnaryExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"enum\": [\n        \"is-null\",\n        \"not-null\",\n        \"is-nan\",\n        \"not-nan\"\n      ]\n    },\n    \"term\": {\n      \"$ref\": \"#/components/schemas/Term\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"term\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-unary-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: UnaryExpression
---
