---
description: Response from a document write operation
layout: schema
name: WriteResponse
properties_list:
- description: ''
  name: ok
  type: boolean
- description: Document ID
  name: id
  type: string
- description: New revision ID
  name: rev
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-write-response-schema.json
slug: apache-couchdb-write-response
source_filename: apache-couchdb-write-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-write-response-schema.json\",\n  \"title\": \"WriteResponse\",\n  \"description\": \"Response from a document write operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Document ID\",\n      \"example\": \"doc001\"\n    },\n    \"rev\": {\n      \"type\": \"string\",\n      \"description\": \"New revision ID\",\n      \"example\": \"1-abc123def456\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-write-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: WriteResponse
---
