---
description: HBase table schema with column family definitions
layout: schema
name: TableSchema
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: ColumnSchema
  type: array
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-tableschema-schema.json
slug: hbase-rest-tableschema
source_filename: hbase-rest-tableschema-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-tableschema-schema.json\",\n  \"title\": \"TableSchema\",\n  \"type\": \"object\",\n  \"description\": \"HBase table schema with column family definitions\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-table\"\n    },\n    \"ColumnSchema\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ColumnFamily\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-tableschema-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: TableSchema
---
