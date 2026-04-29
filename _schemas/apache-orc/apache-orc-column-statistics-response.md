---
description: ColumnStatisticsResponse schema from Apache ORC
layout: schema
name: ColumnStatisticsResponse
properties_list:
- description: ''
  name: filePath
  type: string
- description: ''
  name: statistics
  type: array
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-column-statistics-response-schema.json
slug: apache-orc-column-statistics-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-statistics-response-schema.json\",\n  \"title\": \"ColumnStatisticsResponse\",\n  \"description\": \"ColumnStatisticsResponse schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filePath\": {\n      \"type\": \"string\",\n      \"example\": \"data/sales.orc\"\n    },\n    \"statistics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ColumnStatistics\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-statistics-response-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: ColumnStatisticsResponse
---
