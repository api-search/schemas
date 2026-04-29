---
description: Hive table metadata
layout: schema
name: Table
properties_list:
- description: Table name
  name: tableName
  type: string
- description: Database name
  name: dbName
  type: string
- description: Table type (MANAGED_TABLE, EXTERNAL_TABLE, VIRTUAL_VIEW)
  name: tableType
  type: string
- description: Table description
  name: comment
  type: string
- description: HDFS data location
  name: location
  type: string
- description: Input format class
  name: inputFormat
  type: string
- description: Output format class
  name: outputFormat
  type: string
- description: Approximate number of rows
  name: numRows
  type: integer
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-table-schema.json
slug: hive-webhcat-table
source_filename: hive-webhcat-table-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hive/json-schema/hive-webhcat-table-schema.json\",\n  \"title\": \"Table\",\n  \"type\": \"object\",\n  \"description\": \"Hive table metadata\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Table name\",\n      \"example\": \"sales\"\n    },\n    \"dbName\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\",\n      \"example\": \"mydb\"\n    },\n    \"tableType\": {\n      \"type\": \"string\",\n      \"description\": \"Table type (MANAGED_TABLE, EXTERNAL_TABLE, VIRTUAL_VIEW)\",\n      \"example\": \"MANAGED_TABLE\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Table description\",\n      \"example\": \"Sales transaction data\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"HDFS data location\",\n      \"example\"\
  : \"hdfs://namenode/user/hive/warehouse/mydb.db/sales\"\n    },\n    \"inputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Input format class\",\n      \"example\": \"org.apache.hadoop.hive.ql.io.orc.OrcInputFormat\"\n    },\n    \"outputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Output format class\",\n      \"example\": \"org.apache.hadoop.hive.ql.io.orc.OrcOutputFormat\"\n    },\n    \"numRows\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Approximate number of rows\",\n      \"example\": 1000000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hive/refs/heads/main/json-schema/hive-webhcat-table-schema.json
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Table
---
