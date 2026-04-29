---
description: Region layout for an HBase table
layout: schema
name: TableRegions
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: Region
  type: array
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-tableregions-schema.json
slug: hbase-rest-tableregions
source_filename: hbase-rest-tableregions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-tableregions-schema.json\",\n  \"title\": \"TableRegions\",\n  \"type\": \"object\",\n  \"description\": \"Region layout for an HBase table\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"my-table\"\n    },\n    \"Region\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"format\": \"int64\",\n            \"example\": 1718153645993\n          },\n          \"startKey\": {\n            \"type\": \"string\",\n            \"example\": \"\"\n          },\n          \"endKey\": {\n            \"type\": \"string\",\n            \"example\": \"row500\"\n          },\n          \"location\": {\n            \"type\": \"string\",\n            \"example\": \"regionserver1:16020\"\
  \n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"my-table,,1718153645993.abc123.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-tableregions-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: TableRegions
---
