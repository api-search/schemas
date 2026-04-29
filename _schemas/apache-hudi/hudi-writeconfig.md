---
description: Hudi write operation configuration
layout: schema
name: WriteConfig
properties_list:
- description: Write operation type (UPSERT, INSERT, BULK_INSERT, DELETE)
  name: operation
  type: string
- description: Number of records per write batch
  name: batchSize
  type: integer
- description: Write parallelism (number of partitions)
  name: parallelism
  type: integer
- description: Target file size in bytes for auto bin-packing
  name: smallFileLimit
  type: integer
- description: Whether inline compaction is enabled (MOR tables)
  name: compactionEnabled
  type: boolean
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-writeconfig-schema.json
slug: hudi-writeconfig
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-writeconfig-schema.json\",\n  \"title\": \"WriteConfig\",\n  \"type\": \"object\",\n  \"description\": \"Hudi write operation configuration\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"Write operation type (UPSERT, INSERT, BULK_INSERT, DELETE)\",\n      \"example\": \"UPSERT\"\n    },\n    \"batchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records per write batch\",\n      \"example\": 50000\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"description\": \"Write parallelism (number of partitions)\",\n      \"example\": 100\n    },\n    \"smallFileLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Target file size in bytes for auto bin-packing\",\n      \"example\": 104857600\n    },\n    \"compactionEnabled\": {\n\
  \      \"type\": \"boolean\",\n      \"description\": \"Whether inline compaction is enabled (MOR tables)\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-writeconfig-schema.json
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: WriteConfig
---
