---
description: TableIdentifier schema from Apache Iceberg REST Catalog API
layout: schema
name: TableIdentifier
properties_list:
- description: ''
  name: namespace
  type: object
- description: ''
  name: name
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-table-identifier-schema.json
slug: rest-catalog-open-api-table-identifier
source_filename: rest-catalog-open-api-table-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-identifier-schema.json\",\n  \"title\": \"TableIdentifier\",\n  \"description\": \"TableIdentifier schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"$ref\": \"#/components/schemas/Namespace\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"nullable\": false\n    }\n  },\n  \"required\": [\n    \"namespace\",\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-table-identifier-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TableIdentifier
---
