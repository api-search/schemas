---
description: HBase column family configuration
layout: schema
name: ColumnFamily
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: VERSIONS
  type: string
- description: ''
  name: COMPRESSION
  type: string
- description: ''
  name: BLOOMFILTER
  type: string
- description: ''
  name: TTL
  type: string
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-columnfamily-schema.json
slug: hbase-rest-columnfamily
source_filename: hbase-rest-columnfamily-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-columnfamily-schema.json\",\n  \"title\": \"ColumnFamily\",\n  \"type\": \"object\",\n  \"description\": \"HBase column family configuration\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"cf1\"\n    },\n    \"VERSIONS\": {\n      \"type\": \"string\",\n      \"example\": \"3\"\n    },\n    \"COMPRESSION\": {\n      \"type\": \"string\",\n      \"example\": \"SNAPPY\"\n    },\n    \"BLOOMFILTER\": {\n      \"type\": \"string\",\n      \"example\": \"ROW\"\n    },\n    \"TTL\": {\n      \"type\": \"string\",\n      \"example\": \"2147483647\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-columnfamily-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: ColumnFamily
---
