---
description: Type schema from Apache Iceberg REST Catalog API
layout: schema
name: Type
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-type-schema.json
slug: rest-catalog-open-api-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-type-schema.json\",\n  \"title\": \"Type\",\n  \"description\": \"Type schema from Apache Iceberg REST Catalog API\",\n  \"oneOf\": [\n    {\n      \"$ref\": \"#/components/schemas/PrimitiveType\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/StructType\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/ListType\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/MapType\"\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-type-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Type
---
