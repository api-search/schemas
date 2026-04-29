---
description: NotExpression schema from Apache Iceberg REST Catalog API
layout: schema
name: NotExpression
properties_list:
- description: ''
  name: type
  type: object
- description: ''
  name: child
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-not-expression-schema.json
slug: rest-catalog-open-api-not-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-not-expression-schema.json\",\n  \"title\": \"NotExpression\",\n  \"description\": \"NotExpression schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"$ref\": \"#/components/schemas/ExpressionType\",\n      \"const\": \"not\"\n    },\n    \"child\": {\n      \"$ref\": \"#/components/schemas/Expression\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"child\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-not-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: NotExpression
---
