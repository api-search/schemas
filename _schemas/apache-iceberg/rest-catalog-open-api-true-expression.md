---
description: TrueExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: TrueExpression
properties_list:
- description: ''
  name: type
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-true-expression-schema.json
slug: rest-catalog-open-api-true-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-true-expression-schema.json\",\n  \"title\": \"TrueExpression\",\n  \"description\": \"TrueExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"const\": \"true\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-true-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TrueExpression
---
