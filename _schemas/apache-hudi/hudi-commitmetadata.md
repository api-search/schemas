---
description: Metadata for a completed Hudi commit operation
layout: schema
name: CommitMetadata
properties_list:
- description: Commit timestamp
  name: commitTime
  type: string
- description: Total bytes written
  name: totalWriteBytes
  type: integer
- description: Total records written
  name: totalRecordsWritten
  type: integer
- description: Records updated
  name: totalUpdateRecordsWritten
  type: integer
- description: Records inserted
  name: totalInsertRecordsWritten
  type: integer
- description: Bytes written to storage
  name: totalBytesWritten
  type: integer
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-commitmetadata-schema.json
slug: hudi-commitmetadata
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: CommitMetadata
---
