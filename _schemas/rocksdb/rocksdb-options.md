---
description: Schema representing RocksDB database configuration options controlling storage behavior, compaction, memory usage, and performance tuning.
layout: schema
name: RocksDB Options
properties_list:
- description: If true, the database will be created if it does not exist.
  name: create_if_missing
  type: boolean
- description: If true, an error is raised if the database already exists.
  name: error_if_exists
  type: boolean
- description: If true, the implementation will do aggressive checking of the data it is processing and will stop early if it detects any errors.
  name: paranoid_checks
  type: boolean
- description: Number of open files that can be used by the DB. Value -1 means files are always kept open.
  name: max_open_files
  type: integer
- description: Amount of data to build up in memory (backed by an unsorted log on disk) before converting to a sorted on-disk file. In bytes.
  name: write_buffer_size
  type: integer
- description: The maximum number of write buffers that are built up in memory.
  name: max_write_buffer_number
  type: integer
- description: Target file size for compaction in bytes.
  name: target_file_size_base
  type: integer
- description: Control maximum total data size for a level. Default 256MB.
  name: max_bytes_for_level_base
  type: integer
- description: Compression algorithm used for each level.
  name: compression
  type: string
- description: 'The compaction style: level-based, universal, FIFO, or none.'
  name: compaction_style
  type: string
- description: Number of levels for this database.
  name: num_levels
  type: integer
- description: Number of files to trigger level-0 compaction.
  name: level0_file_num_compaction_trigger
  type: integer
- description: Maximum number of concurrent background jobs (compactions and flushes).
  name: max_background_jobs
  type: integer
- description: Use O_DIRECT for background flush and compaction I/O.
  name: use_direct_io_for_flush_and_compaction
  type: boolean
- description: Enable BlobDB for storing large values separately from the LSM tree.
  name: enable_blob_files
  type: boolean
- description: Values at or above this threshold will be stored in blob files. In bytes.
  name: min_blob_size
  type: integer
- description: Compression algorithm for blob files.
  name: blob_compression_type
  type: string
- description: Time to live in seconds for keys. 0 means no TTL.
  name: ttl
  type: integer
provider_name: RocksDB
provider_slug: rocksdb
schema_file: json-schema/rocksdb-options-schema.json
slug: rocksdb-options
source_filename: rocksdb-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/rocksdb/json-schema/rocksdb-options-schema.json\",\n  \"title\": \"RocksDB Options\",\n  \"description\": \"Schema representing RocksDB database configuration options controlling storage behavior, compaction, memory usage, and performance tuning.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"create_if_missing\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the database will be created if it does not exist.\",\n      \"default\": false\n    },\n    \"error_if_exists\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, an error is raised if the database already exists.\",\n      \"default\": false\n    },\n    \"paranoid_checks\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, the implementation will do aggressive checking of the data it is processing and will stop early if it detects any errors.\"\
  ,\n      \"default\": false\n    },\n    \"max_open_files\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of open files that can be used by the DB. Value -1 means files are always kept open.\",\n      \"default\": -1\n    },\n    \"write_buffer_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Amount of data to build up in memory (backed by an unsorted log on disk) before converting to a sorted on-disk file. In bytes.\",\n      \"default\": 67108864\n    },\n    \"max_write_buffer_number\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of write buffers that are built up in memory.\",\n      \"default\": 2\n    },\n    \"target_file_size_base\": {\n      \"type\": \"integer\",\n      \"description\": \"Target file size for compaction in bytes.\",\n      \"default\": 67108864\n    },\n    \"max_bytes_for_level_base\": {\n      \"type\": \"integer\",\n      \"description\": \"Control maximum total data size for a level. Default\
  \ 256MB.\",\n      \"default\": 268435456\n    },\n    \"compression\": {\n      \"type\": \"string\",\n      \"enum\": [\"no_compression\", \"snappy\", \"zlib\", \"bzip2\", \"lz4\", \"lz4hc\", \"xpress\", \"zstd\"],\n      \"description\": \"Compression algorithm used for each level.\",\n      \"default\": \"snappy\"\n    },\n    \"compaction_style\": {\n      \"type\": \"string\",\n      \"enum\": [\"level\", \"universal\", \"fifo\", \"none\"],\n      \"description\": \"The compaction style: level-based, universal, FIFO, or none.\",\n      \"default\": \"level\"\n    },\n    \"num_levels\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of levels for this database.\",\n      \"default\": 7\n    },\n    \"level0_file_num_compaction_trigger\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of files to trigger level-0 compaction.\",\n      \"default\": 4\n    },\n    \"max_background_jobs\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum\
  \ number of concurrent background jobs (compactions and flushes).\",\n      \"default\": 2\n    },\n    \"use_direct_io_for_flush_and_compaction\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use O_DIRECT for background flush and compaction I/O.\",\n      \"default\": false\n    },\n    \"enable_blob_files\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable BlobDB for storing large values separately from the LSM tree.\",\n      \"default\": false\n    },\n    \"min_blob_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Values at or above this threshold will be stored in blob files. In bytes.\",\n      \"default\": 0\n    },\n    \"blob_compression_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"no_compression\", \"snappy\", \"zlib\", \"bzip2\", \"lz4\", \"lz4hc\", \"zstd\"],\n      \"description\": \"Compression algorithm for blob files.\",\n      \"default\": \"no_compression\"\n    },\n    \"ttl\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Time to live in seconds for keys. 0 means no TTL.\",\n      \"default\": 0\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rocksdb/refs/heads/main/json-schema/rocksdb-options-schema.json
tags:
- RocksDB
- Key-Value Store
- Embedded Database
- Storage Engine
- Open Source
title: RocksDB Options
---
