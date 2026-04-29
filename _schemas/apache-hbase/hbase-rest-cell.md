---
description: Single HBase cell with column and value
layout: schema
name: Cell
properties_list:
- description: ''
  name: column
  type: string
- description: ''
  name: timestamp
  type: integer
- description: ''
  name: $
  type: string
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-cell-schema.json
slug: hbase-rest-cell
source_filename: hbase-rest-cell-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-cell-schema.json\",\n  \"title\": \"Cell\",\n  \"type\": \"object\",\n  \"description\": \"Single HBase cell with column and value\",\n  \"properties\": {\n    \"column\": {\n      \"type\": \"string\",\n      \"example\": \"Y2YxOnF1YWw=\"\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1718153645993\n    },\n    \"$\": {\n      \"type\": \"string\",\n      \"example\": \"dmFsdWU=\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-cell-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: Cell
---
