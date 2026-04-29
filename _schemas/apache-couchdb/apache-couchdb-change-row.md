---
description: A single change record in the changes feed
layout: schema
name: ChangeRow
properties_list:
- description: Update sequence number
  name: seq
  type: string
- description: Document ID that was changed
  name: id
  type: string
- description: ''
  name: changes
  type: array
- description: True if this change is a deletion
  name: deleted
  type: boolean
- description: A CouchDB document with system fields and user-defined fields
  name: doc
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-change-row-schema.json
slug: apache-couchdb-change-row
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-change-row-schema.json\",\n  \"title\": \"ChangeRow\",\n  \"description\": \"A single change record in the changes feed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"seq\": {\n      \"type\": \"string\",\n      \"description\": \"Update sequence number\",\n      \"example\": \"5000-abc123\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document ID that was changed\",\n      \"example\": \"doc001\"\n    },\n    \"changes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rev\": {\n            \"type\": \"string\",\n            \"example\": \"2-def456\"\n          }\n        }\n      }\n    },\n    \"deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if this\
  \ change is a deletion\",\n      \"example\": false\n    },\n    \"doc\": {\n      \"title\": \"Document\",\n      \"type\": \"object\",\n      \"description\": \"A CouchDB document with system fields and user-defined fields\",\n      \"properties\": {\n        \"_id\": {\n          \"type\": \"string\",\n          \"description\": \"Document ID\",\n          \"example\": \"doc001\"\n        },\n        \"_rev\": {\n          \"type\": \"string\",\n          \"description\": \"Current revision ID (major-hash format)\",\n          \"example\": \"1-abc123def456\"\n        },\n        \"_deleted\": {\n          \"type\": \"boolean\",\n          \"description\": \"Present and true for deleted (tombstone) documents\",\n          \"example\": false\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-change-row-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ChangeRow
---
