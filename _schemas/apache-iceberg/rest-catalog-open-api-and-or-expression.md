---
description: AndOrExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: AndOrExpression
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: left
  type: object
- description: ''
  name: right
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-and-or-expression-schema.json
slug: rest-catalog-open-api-and-or-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-and-or-expression-schema.json\",\n  \"title\": \"AndOrExpression\",\n  \"description\": \"AndOrExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"enum\": [\n        \"and\",\n        \"or\"\n      ]\n    },\n    \"left\": {\n      \"$ref\": \"#/components/schemas/Expression\"\n    },\n    \"right\": {\n      \"$ref\": \"#/components/schemas/Expression\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"left\",\n    \"right\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-and-or-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: AndOrExpression
---
