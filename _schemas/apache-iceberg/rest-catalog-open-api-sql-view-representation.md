---
description: SQLViewRepresentation schema from Apache Iceberg REST Catalog API
layout: schema
name: SQLViewRepresentation
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: sql
  type: string
- description: ''
  name: dialect
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-sql-view-representation-schema.json
slug: rest-catalog-open-api-sql-view-representation
source_filename: rest-catalog-open-api-sql-view-representation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sql-view-representation-schema.json\",\n  \"title\": \"SQLViewRepresentation\",\n  \"description\": \"SQLViewRepresentation schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"sql\": {\n      \"type\": \"string\"\n    },\n    \"dialect\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"sql\",\n    \"dialect\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sql-view-representation-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SQLViewRepresentation
---
