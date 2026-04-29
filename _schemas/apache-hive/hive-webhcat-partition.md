---
description: Hive table partition
layout: schema
name: Partition
properties_list:
- description: Table name
  name: tableName
  type: string
- description: Database name
  name: dbName
  type: string
- description: Partition key values
  name: values
  type: array
- description: Partition HDFS location
  name: location
  type: string
- description: Approximate row count
  name: numRows
  type: integer
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-partition-schema.json
slug: hive-webhcat-partition
source_filename: hive-webhcat-partition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-partition-schema.json\",\n  \"title\": \"Partition\",\n  \"type\": \"object\",\n  \"description\": \"Hive table partition\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Table name\",\n      \"example\": \"sales\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\",\n      \"example\": \"mydb\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Partition key values\",\n      \"example\": [\n        \"2024-01\",\n        \"US\"\n      ]\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Partition HDFS location\",\n      \"example\": \"hdfs://namenode/user/hive/warehouse/mydb.db/sales/dt=2024-01/country=US\"\n   \
  \ },\n    \"numRows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Approximate row count\",\n      \"example\": 50000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-partition-schema.json
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Partition
---
