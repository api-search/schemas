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
