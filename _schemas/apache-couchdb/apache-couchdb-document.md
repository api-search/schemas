---
description: A CouchDB document with system fields and user-defined fields
layout: schema
name: Document
properties_list:
- description: Document ID
  name: _id
  type: string
- description: Current revision ID (major-hash format)
  name: _rev
  type: string
- description: Present and true for deleted (tombstone) documents
  name: _deleted
  type: boolean
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-document-schema.json
slug: apache-couchdb-document
source_filename: apache-couchdb-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-document-schema.json\",\n  \"title\": \"Document\",\n  \"description\": \"A CouchDB document with system fields and user-defined fields\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Document ID\",\n      \"example\": \"doc001\"\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Current revision ID (major-hash format)\",\n      \"example\": \"1-abc123def456\"\n    },\n    \"_deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Present and true for deleted (tombstone) documents\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-document-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: Document
---
