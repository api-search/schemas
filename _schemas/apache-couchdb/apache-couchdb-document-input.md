---
description: Input for creating or updating a CouchDB document
layout: schema
name: DocumentInput
properties_list:
- description: Optional document ID (auto-generated if omitted for POST)
  name: _id
  type: string
- description: Required for updates — current revision ID
  name: _rev
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-document-input-schema.json
slug: apache-couchdb-document-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-document-input-schema.json\",\n  \"title\": \"DocumentInput\",\n  \"description\": \"Input for creating or updating a CouchDB document\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Optional document ID (auto-generated if omitted for POST)\",\n      \"example\": \"doc001\"\n    },\n    \"_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Required for updates \\u2014 current revision ID\",\n      \"example\": \"1-abc123def456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-document-input-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DocumentInput
---
