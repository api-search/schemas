---
description: SortOrder schema from Apache Iceberg REST Catalog API
layout: schema
name: SortOrder
properties_list:
- description: ''
  name: order-id
  type: integer
- description: ''
  name: fields
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-sort-order-schema.json
slug: rest-catalog-open-api-sort-order
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sort-order-schema.json\",\n  \"title\": \"SortOrder\",\n  \"description\": \"SortOrder schema from Apache Iceberg REST Catalog API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order-id\": {\n      \"type\": \"integer\",\n      \"readOnly\": true\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SortField\"\n      }\n    }\n  },\n  \"required\": [\n    \"order-id\",\n    \"fields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-sort-order-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SortOrder
---
