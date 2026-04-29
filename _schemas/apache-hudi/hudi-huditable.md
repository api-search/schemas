---
description: Apache Hudi table metadata and configuration
layout: schema
name: HudiTable
properties_list:
- description: Hudi table name
  name: tableName
  type: string
- description: HDFS or S3 base path for the table
  name: basePath
  type: string
- description: Table type (COPY_ON_WRITE or MERGE_ON_READ)
  name: tableType
  type: string
- description: Avro schema string for the table
  name: schema
  type: string
- description: Field used for deduplication ordering
  name: preCombineField
  type: string
- description: Field used as record key
  name: recordKeyField
  type: string
- description: Field used for partitioning
  name: partitionPathField
  type: string
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-huditable-schema.json
slug: hudi-huditable
source_filename: hudi-huditable-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-huditable-schema.json\",\n  \"title\": \"HudiTable\",\n  \"type\": \"object\",\n  \"description\": \"Apache Hudi table metadata and configuration\",\n  \"properties\": {\n    \"tableName\": {\n      \"type\": \"string\",\n      \"description\": \"Hudi table name\",\n      \"example\": \"orders\"\n    },\n    \"basePath\": {\n      \"type\": \"string\",\n      \"description\": \"HDFS or S3 base path for the table\",\n      \"example\": \"s3://my-bucket/hudi/orders\"\n    },\n    \"tableType\": {\n      \"type\": \"string\",\n      \"description\": \"Table type (COPY_ON_WRITE or MERGE_ON_READ)\",\n      \"example\": \"COPY_ON_WRITE\"\n    },\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"Avro schema string for the table\",\n      \"example\": \"{}\"\n    },\n    \"preCombineField\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Field used for deduplication ordering\",\n      \"example\": \"ts\"\n    },\n    \"recordKeyField\": {\n      \"type\": \"string\",\n      \"description\": \"Field used as record key\",\n      \"example\": \"order_id\"\n    },\n    \"partitionPathField\": {\n      \"type\": \"string\",\n      \"description\": \"Field used for partitioning\",\n      \"example\": \"order_date\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-huditable-schema.json
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: HudiTable
---
