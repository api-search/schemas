---
description: HBase scanner configuration for table scans
layout: schema
name: Scanner
properties_list:
- description: ''
  name: startRow
  type: string
- description: ''
  name: endRow
  type: string
- description: ''
  name: batch
  type: integer
- description: ''
  name: maxVersions
  type: integer
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-scanner-schema.json
slug: hbase-rest-scanner
source_filename: hbase-rest-scanner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-scanner-schema.json\",\n  \"title\": \"Scanner\",\n  \"type\": \"object\",\n  \"description\": \"HBase scanner configuration for table scans\",\n  \"properties\": {\n    \"startRow\": {\n      \"type\": \"string\",\n      \"example\": \"cm93MQ==\"\n    },\n    \"endRow\": {\n      \"type\": \"string\",\n      \"example\": \"cm93Mg==\"\n    },\n    \"batch\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"maxVersions\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-scanner-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: Scanner
---
