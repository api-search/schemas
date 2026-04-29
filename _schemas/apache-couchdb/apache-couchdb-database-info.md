---
description: Information about a CouchDB database
layout: schema
name: DatabaseInfo
properties_list:
- description: Database name
  name: db_name
  type: string
- description: Number of non-deleted documents
  name: doc_count
  type: integer
- description: Number of deleted documents (tombstones)
  name: doc_del_count
  type: integer
- description: Current update sequence
  name: update_seq
  type: string
- description: ''
  name: sizes
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-database-info-schema.json
slug: apache-couchdb-database-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-database-info-schema.json\",\n  \"title\": \"DatabaseInfo\",\n  \"description\": \"Information about a CouchDB database\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"db_name\": {\n      \"type\": \"string\",\n      \"description\": \"Database name\",\n      \"example\": \"mydb\"\n    },\n    \"doc_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of non-deleted documents\",\n      \"example\": 1250\n    },\n    \"doc_del_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of deleted documents (tombstones)\",\n      \"example\": 42\n    },\n    \"update_seq\": {\n      \"type\": \"string\",\n      \"description\": \"Current update sequence\",\n      \"example\": \"5000-abc123\"\n    },\n    \"sizes\": {\n      \"type\": \"object\",\n\
  \      \"properties\": {\n        \"file\": {\n          \"type\": \"integer\",\n          \"description\": \"Disk file size in bytes\",\n          \"example\": 4096000\n        },\n        \"external\": {\n          \"type\": \"integer\",\n          \"description\": \"Uncompressed data size in bytes\",\n          \"example\": 2048000\n        },\n        \"active\": {\n          \"type\": \"integer\",\n          \"description\": \"Active data size in bytes\",\n          \"example\": 3000000\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-database-info-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DatabaseInfo
---
