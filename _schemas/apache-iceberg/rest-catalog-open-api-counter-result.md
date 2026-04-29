---
description: CounterResult schema from Apache Iceberg REST Catalog API
layout: schema
name: CounterResult
properties_list:
- description: ''
  name: unit
  type: string
- description: ''
  name: value
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-counter-result-schema.json
slug: rest-catalog-open-api-counter-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-counter-result-schema.json\",\n  \"title\": \"CounterResult\",\n  \"description\": \"CounterResult schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"unit\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-counter-result-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CounterResult
---
