---
description: Request body for _bulk_docs
layout: schema
name: BulkDocsRequest
properties_list:
- description: Array of documents to create, update, or delete
  name: docs
  type: array
- description: If false, allow insertion of conflicting revisions (for replication)
  name: new_edits
  type: boolean
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-bulk-docs-request-schema.json
slug: apache-couchdb-bulk-docs-request
source_filename: apache-couchdb-bulk-docs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-bulk-docs-request-schema.json\",\n  \"title\": \"BulkDocsRequest\",\n  \"description\": \"Request body for _bulk_docs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"docs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"DocumentInput\",\n        \"type\": \"object\",\n        \"description\": \"Input for creating or updating a CouchDB document\",\n        \"properties\": {\n          \"_id\": {\n            \"type\": \"string\",\n            \"description\": \"Optional document ID (auto-generated if omitted for POST)\",\n            \"example\": \"doc001\"\n          },\n          \"_rev\": {\n            \"type\": \"string\",\n            \"description\": \"Required for updates \\u2014 current revision ID\",\n            \"example\": \"1-abc123def456\"\n\
  \          }\n        }\n      },\n      \"description\": \"Array of documents to create, update, or delete\"\n    },\n    \"new_edits\": {\n      \"type\": \"boolean\",\n      \"description\": \"If false, allow insertion of conflicting revisions (for replication)\",\n      \"default\": true,\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-bulk-docs-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: BulkDocsRequest
---
