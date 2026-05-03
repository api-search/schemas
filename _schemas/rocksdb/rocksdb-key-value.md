---
description: Schema representing a key-value entry in a RocksDB database, including optional column family and metadata.
layout: schema
name: RocksDB Key-Value Entry
properties_list:
- description: The key as a string or base64-encoded byte string for binary keys.
  name: key
  type: string
- description: The value associated with the key. Can be a string, object, or base64 bytes.
  name: value
  type: object
- description: Name of the column family containing this entry. Defaults to 'default'.
  name: column_family
  type: string
- description: Internal RocksDB sequence number at which this entry was written.
  name: sequence_number
  type: integer
- description: Type of the RocksDB write operation.
  name: type
  type: string
- description: Timestamp of the write operation (when user-defined timestamps are enabled).
  name: timestamp
  type: string
- description: Time-to-live in seconds from the creation time. Key expires after this duration.
  name: ttl_seconds
  type: integer
provider_name: RocksDB
provider_slug: rocksdb
schema_file: json-schema/rocksdb-key-value-schema.json
slug: rocksdb-key-value
source_filename: rocksdb-key-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/rocksdb/json-schema/rocksdb-key-value-schema.json\",\n  \"title\": \"RocksDB Key-Value Entry\",\n  \"description\": \"Schema representing a key-value entry in a RocksDB database, including optional column family and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"key\", \"value\"],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key as a string or base64-encoded byte string for binary keys.\",\n      \"examples\": [\"user:12345\", \"session:abc123\"]\n    },\n    \"value\": {\n      \"description\": \"The value associated with the key. Can be a string, object, or base64 bytes.\",\n      \"examples\": [\"{\\\"name\\\": \\\"Alice\\\"}\", \"binary-data-base64\"]\n    },\n    \"column_family\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the column family containing this entry. Defaults\
  \ to 'default'.\",\n      \"default\": \"default\"\n    },\n    \"sequence_number\": {\n      \"type\": \"integer\",\n      \"description\": \"Internal RocksDB sequence number at which this entry was written.\",\n      \"minimum\": 0\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"put\", \"delete\", \"merge\", \"single_delete\"],\n      \"description\": \"Type of the RocksDB write operation.\",\n      \"default\": \"put\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the write operation (when user-defined timestamps are enabled).\"\n    },\n    \"ttl_seconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Time-to-live in seconds from the creation time. Key expires after this duration.\",\n      \"minimum\": 0\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rocksdb/refs/heads/main/json-schema/rocksdb-key-value-schema.json
tags:
- RocksDB
- Key-Value Store
- Embedded Database
- Storage Engine
- Open Source
title: RocksDB Key-Value Entry
---
