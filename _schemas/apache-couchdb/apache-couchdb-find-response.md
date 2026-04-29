---
description: Mango query results
layout: schema
name: FindResponse
properties_list:
- description: Array of matching documents
  name: docs
  type: array
- description: Bookmark for retrieving the next set of results
  name: bookmark
  type: string
- description: Warning if query is not optimally indexed
  name: warning
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-find-response-schema.json
slug: apache-couchdb-find-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-find-response-schema.json\",\n  \"title\": \"FindResponse\",\n  \"description\": \"Mango query results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"docs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"Document\",\n        \"type\": \"object\",\n        \"description\": \"A CouchDB document with system fields and user-defined fields\",\n        \"properties\": {\n          \"_id\": {\n            \"type\": \"string\",\n            \"description\": \"Document ID\",\n            \"example\": \"doc001\"\n          },\n          \"_rev\": {\n            \"type\": \"string\",\n            \"description\": \"Current revision ID (major-hash format)\",\n            \"example\": \"1-abc123def456\"\n          },\n          \"_deleted\": {\n            \"type\":\
  \ \"boolean\",\n            \"description\": \"Present and true for deleted (tombstone) documents\",\n            \"example\": false\n          }\n        }\n      },\n      \"description\": \"Array of matching documents\"\n    },\n    \"bookmark\": {\n      \"type\": \"string\",\n      \"description\": \"Bookmark for retrieving the next set of results\",\n      \"example\": \"g1AAAABleJzLYWBg\"\n    },\n    \"warning\": {\n      \"type\": \"string\",\n      \"description\": \"Warning if query is not optimally indexed\",\n      \"example\": \"No matching index found, create an index to optimize query time.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-find-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: FindResponse
---
