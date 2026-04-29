---
description: Expression schema from Apache Iceberg REST Catalog API
layout: schema
name: Expression
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-expression-schema.json
slug: rest-catalog-open-api-expression
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-expression-schema.json\",\n  \"title\": \"Expression\",\n  \"description\": \"Expression schema from Apache Iceberg REST Catalog API\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/TrueExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/FalseExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/AndOrExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/NotExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/SetExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/LiteralExpression\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/UnaryExpression\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-expression-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Expression
---
