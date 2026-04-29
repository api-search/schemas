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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-hudi/json-schema/hudi-commitmetadata-schema.json\",\n  \"title\": \"CommitMetadata\",\n  \"type\": \"object\",\n  \"description\": \"Metadata for a completed Hudi commit operation\",\n  \"properties\": {\n    \"commitTime\": {\n      \"type\": \"string\",\n      \"description\": \"Commit timestamp\",\n      \"example\": \"20240101120000000\"\n    },\n    \"totalWriteBytes\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total bytes written\",\n      \"example\": 52428800\n    },\n    \"totalRecordsWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Total records written\",\n      \"example\": 100000\n    },\n    \"totalUpdateRecordsWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Records updated\",\n      \"example\": 30000\n\
  \    },\n    \"totalInsertRecordsWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Records inserted\",\n      \"example\": 70000\n    },\n    \"totalBytesWritten\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Bytes written to storage\",\n      \"example\": 52428800\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-hudi/refs/heads/main/json-schema/hudi-commitmetadata-schema.json
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
