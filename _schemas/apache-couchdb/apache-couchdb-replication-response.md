---
description: Result of a replication request
layout: schema
name: ReplicationResponse
properties_list:
- description: ''
  name: ok
  type: boolean
- description: ''
  name: session_id
  type: string
- description: ''
  name: source_last_seq
  type: string
- description: ''
  name: history
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-replication-response-schema.json
slug: apache-couchdb-replication-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-replication-response-schema.json\",\n  \"title\": \"ReplicationResponse\",\n  \"description\": \"Result of a replication request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"session_id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123def456\"\n    },\n    \"source_last_seq\": {\n      \"type\": \"string\",\n      \"example\": \"5000-abc123\"\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"session_id\": {\n            \"type\": \"string\"\n          },\n          \"docs_written\": {\n            \"type\": \"integer\"\n          },\n          \"doc_write_failures\": {\n            \"type\": \"\
  integer\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-replication-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ReplicationResponse
---
