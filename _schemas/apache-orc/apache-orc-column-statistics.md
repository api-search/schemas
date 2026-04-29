---
description: ColumnStatistics schema from Apache ORC
layout: schema
name: ColumnStatistics
properties_list:
- description: ''
  name: columnIndex
  type: integer
- description: ''
  name: columnName
  type: string
- description: ''
  name: valueCount
  type: integer
- description: ''
  name: nullCount
  type: integer
- description: ''
  name: hasMinimum
  type: boolean
- description: ''
  name: minimum
  type: string
- description: ''
  name: maximum
  type: string
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-column-statistics-schema.json
slug: apache-orc-column-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-statistics-schema.json\",\n  \"title\": \"ColumnStatistics\",\n  \"description\": \"ColumnStatistics schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"columnIndex\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"columnName\": {\n      \"type\": \"string\",\n      \"example\": \"customer_id\"\n    },\n    \"valueCount\": {\n      \"type\": \"integer\",\n      \"example\": 999500\n    },\n    \"nullCount\": {\n      \"type\": \"integer\",\n      \"example\": 500\n    },\n    \"hasMinimum\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"minimum\": {\n      \"type\": \"string\",\n      \"example\": \"1\"\n    },\n    \"maximum\": {\n      \"type\": \"string\",\n      \"example\": \"999999\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-statistics-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: ColumnStatistics
---
