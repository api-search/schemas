---
description: Set of HBase cells grouped by row
layout: schema
name: CellSet
properties_list:
- description: ''
  name: Row
  type: array
provider_name: Apache HBase
provider_slug: apache-hbase
schema_file: json-schema/hbase-rest-cellset-schema.json
slug: hbase-rest-cellset
source_filename: hbase-rest-cellset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hbase/json-schema/hbase-rest-cellset-schema.json\",\n  \"title\": \"CellSet\",\n  \"type\": \"object\",\n  \"description\": \"Set of HBase cells grouped by row\",\n  \"properties\": {\n    \"Row\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"example\": \"cm93a2V5MQ==\"\n          },\n          \"Cell\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/definitions/Cell\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hbase/refs/heads/main/json-schema/hbase-rest-cellset-schema.json
tags:
- Apache
- Big Data
- Bigtable
- Database
- Hadoop
- NoSQL
- Open Source
- Wide Column
title: CellSet
---
