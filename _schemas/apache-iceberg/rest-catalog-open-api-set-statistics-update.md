---
description: SetStatisticsUpdate schema from Apache Iceberg REST Catalog API
layout: schema
name: SetStatisticsUpdate
properties_list:
- description: ''
  name: action
  type: string
- description: This optional field is **DEPRECATED for REMOVAL** since it contains redundant information. Clients should use the `statistics.snapshot-id` field instead.
  name: snapshot-id
  type: integer
- description: ''
  name: statistics
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-set-statistics-update-schema.json
slug: rest-catalog-open-api-set-statistics-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-statistics-update-schema.json\",\n  \"title\": \"SetStatisticsUpdate\",\n  \"description\": \"SetStatisticsUpdate schema from Apache Iceberg REST Catalog API\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"const\": \"set-statistics\"\n    },\n    \"snapshot-id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"deprecated\": true,\n      \"description\": \"This optional field is **DEPRECATED for REMOVAL** since it contains redundant information. Clients should use the `statistics.snapshot-id` field instead.\"\n    },\n    \"statistics\": {\n      \"$ref\": \"#/components/schemas/StatisticsFile\"\n    }\n  },\n  \"required\": [\n    \"statistics\"\n  ],\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/BaseUpdate\"\
  \n    }\n  ],\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-set-statistics-update-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: SetStatisticsUpdate
---
