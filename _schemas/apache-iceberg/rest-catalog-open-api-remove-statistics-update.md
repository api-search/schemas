---
description: RemoveStatisticsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: RemoveStatisticsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: snapshot-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-remove-statistics-update-schema.json
slug: rest-catalog-open-api-remove-statistics-update
source_filename: rest-catalog-open-api-remove-statistics-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-statistics-update-schema.json\",\n  \"title\": \"RemoveStatisticsUpdate\",\n  \"description\": \"RemoveStatisticsUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"remove-statistics\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  },\n  \"required\": [\n    \"snapshot-id\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-remove-statistics-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: RemoveStatisticsUpdate
---
