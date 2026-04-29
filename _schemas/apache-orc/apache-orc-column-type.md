---
description: ColumnType schema from Apache ORC
layout: schema
name: ColumnType
properties_list:
- description: Column name
  name: name
  type: string
- description: ORC type
  name: type
  type: string
- description: ''
  name: nullable
  type: boolean
- description: ''
  name: children
  type: array
provider_name: Apache ORC
provider_slug: apache-orc
schema_file: json-schema/apache-orc-column-type-schema.json
slug: apache-orc-column-type
source_filename: apache-orc-column-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-type-schema.json\",\n  \"title\": \"ColumnType\",\n  \"description\": \"ColumnType schema from Apache ORC\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Column name\",\n      \"example\": \"customer_id\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"ORC type\",\n      \"example\": \"int\",\n      \"enum\": [\n        \"boolean\",\n        \"tinyint\",\n        \"smallint\",\n        \"int\",\n        \"bigint\",\n        \"float\",\n        \"double\",\n        \"string\",\n        \"binary\",\n        \"timestamp\",\n        \"date\",\n        \"decimal\",\n        \"varchar\",\n        \"char\",\n        \"list\",\n        \"map\",\n        \"struct\",\n        \"union\"\n      ]\n\
  \    },\n    \"nullable\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"children\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ColumnType\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-orc/refs/heads/main/json-schema/apache-orc-column-type-schema.json
tags:
- Big Data
- Columnar Storage
- Compression
- File Format
- Hadoop
- Apache
- Open Source
title: ColumnType
---
