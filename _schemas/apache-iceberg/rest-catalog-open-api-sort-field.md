---
description: SortField schema from Apache Iceberg REST Catalog API
layout: schema
name: SortField
properties_list:
- description: ''
  name: source-id
  type: integer
- description: ''
  name: transform
  type: object
- description: ''
  name: direction
  type: object
- description: ''
  name: null-order
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-sort-field-schema.json
slug: rest-catalog-open-api-sort-field
source_filename: rest-catalog-open-api-sort-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sort-field-schema.json\",\n  \"title\": \"SortField\",\n  \"description\": \"SortField schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source-id\": {\n      \"type\": \"integer\"\n    },\n    \"transform\": {\n      \"$ref\": \"#/components/schemas/Transform\"\n    },\n    \"direction\": {\n      \"$ref\": \"#/components/schemas/SortDirection\"\n    },\n    \"null-order\": {\n      \"$ref\": \"#/components/schemas/NullOrder\"\n    }\n  },\n  \"required\": [\n    \"source-id\",\n    \"transform\",\n    \"direction\",\n    \"null-order\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sort-field-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SortField
---
