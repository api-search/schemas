---
description: ListTablesResponse schema from Apache Iceberg REST Catalog API
layout: schema
name: ListTablesResponse
properties_list:
- description: ''
  name: next-page-token
  type: object
- description: ''
  name: identifiers
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-list-tables-response-schema.json
slug: rest-catalog-open-api-list-tables-response
source_filename: rest-catalog-open-api-list-tables-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-list-tables-response-schema.json\",\n  \"title\": \"ListTablesResponse\",\n  \"description\": \"ListTablesResponse schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"next-page-token\": {\n      \"$ref\": \"#/components/schemas/PageToken\"\n    },\n    \"identifiers\": {\n      \"type\": \"array\",\n      \"uniqueItems\": true,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TableIdentifier\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-list-tables-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: ListTablesResponse
---
