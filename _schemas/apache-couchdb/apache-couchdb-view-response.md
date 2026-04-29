---
description: MapReduce view query results
layout: schema
name: ViewResponse
properties_list:
- description: Total number of rows in the view
  name: total_rows
  type: integer
- description: Number of skipped rows
  name: offset
  type: integer
- description: ''
  name: rows
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-view-response-schema.json
slug: apache-couchdb-view-response
source_filename: apache-couchdb-view-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-view-response-schema.json\",\n  \"title\": \"ViewResponse\",\n  \"description\": \"MapReduce view query results\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows in the view\",\n      \"example\": 150\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of skipped rows\",\n      \"example\": 0\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"doc001\"\n          },\n          \"key\": {\n            \"description\": \"Emitted key from the map function\",\n            \"example\": \"active\"\n\
  \          },\n          \"value\": {\n            \"description\": \"Emitted value from the map or reduce function\",\n            \"example\": 1\n          },\n          \"doc\": {\n            \"title\": \"Document\",\n            \"type\": \"object\",\n            \"description\": \"A CouchDB document with system fields and user-defined fields\",\n            \"properties\": {\n              \"_id\": {\n                \"type\": \"string\",\n                \"description\": \"Document ID\",\n                \"example\": \"doc001\"\n              },\n              \"_rev\": {\n                \"type\": \"string\",\n                \"description\": \"Current revision ID (major-hash format)\",\n                \"example\": \"1-abc123def456\"\n              },\n              \"_deleted\": {\n                \"type\": \"boolean\",\n                \"description\": \"Present and true for deleted (tombstone) documents\",\n                \"example\": false\n              }\n            }\n\
  \          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-view-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ViewResponse
---
