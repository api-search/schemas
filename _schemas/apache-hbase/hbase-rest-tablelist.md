---
description: List of HBase tables
layout: schema
name: TableList
properties_list:
- description: Array of table names
  name: table
  type: array
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-tablelist-schema.json
slug: hbase-rest-tablelist
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-tablelist-schema.json\",\n  \"title\": \"TableList\",\n  \"type\": \"object\",\n  \"description\": \"List of HBase tables\",\n  \"properties\": {\n    \"table\": {\n      \"type\": \"array\",\n      \"description\": \"Array of table names\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"my-table\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-tablelist-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: TableList
---
