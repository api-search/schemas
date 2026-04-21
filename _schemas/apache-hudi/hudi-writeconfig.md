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
