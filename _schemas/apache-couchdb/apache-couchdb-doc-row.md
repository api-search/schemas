---
description: A row in an _all_docs response
layout: schema
name: DocRow
properties_list:
- description: Document ID
  name: id
  type: string
- description: Row key
  name: key
  type: string
- description: Row value containing revision info
  name: value
  type: object
- description: A CouchDB document with system fields and user-defined fields
  name: doc
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-doc-row-schema.json
slug: apache-couchdb-doc-row
source_filename: apache-couchdb-doc-row-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-doc-row-schema.json\",\n  \"title\": \"DocRow\",\n  \"description\": \"A row in an _all_docs response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document ID\",\n      \"example\": \"doc001\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Row key\",\n      \"example\": \"doc001\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"Row value containing revision info\",\n      \"properties\": {\n        \"rev\": {\n          \"type\": \"string\",\n          \"example\": \"1-abc123\"\n        }\n      }\n    },\n    \"doc\": {\n      \"title\": \"Document\",\n      \"type\": \"object\",\n      \"description\": \"A CouchDB document with system fields and user-defined\
  \ fields\",\n      \"properties\": {\n        \"_id\": {\n          \"type\": \"string\",\n          \"description\": \"Document ID\",\n          \"example\": \"doc001\"\n        },\n        \"_rev\": {\n          \"type\": \"string\",\n          \"description\": \"Current revision ID (major-hash format)\",\n          \"example\": \"1-abc123def456\"\n        },\n        \"_deleted\": {\n          \"type\": \"boolean\",\n          \"description\": \"Present and true for deleted (tombstone) documents\",\n          \"example\": false\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-doc-row-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DocRow
---
