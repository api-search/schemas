---
description: Replication task parameters
layout: schema
name: ReplicationRequest
properties_list:
- description: Source database URL or name
  name: source
  type: string
- description: Target database URL or name
  name: target
  type: string
- description: Keep the replication running continuously
  name: continuous
  type: boolean
- description: Create the target database if it does not exist
  name: create_target
  type: boolean
- description: Filter function name to limit replicated documents
  name: filter
  type: string
- description: List of document IDs to replicate
  name: doc_ids
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-replication-request-schema.json
slug: apache-couchdb-replication-request
source_filename: apache-couchdb-replication-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-replication-request-schema.json\",\n  \"title\": \"ReplicationRequest\",\n  \"description\": \"Replication task parameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source database URL or name\",\n      \"example\": \"http://localhost:5984/sourcedb\"\n    },\n    \"target\": {\n      \"type\": \"string\",\n      \"description\": \"Target database URL or name\",\n      \"example\": \"http://remotehost:5984/targetdb\"\n    },\n    \"continuous\": {\n      \"type\": \"boolean\",\n      \"description\": \"Keep the replication running continuously\",\n      \"default\": false,\n      \"example\": false\n    },\n    \"create_target\": {\n      \"type\": \"boolean\",\n      \"description\": \"Create the target database\
  \ if it does not exist\",\n      \"default\": false,\n      \"example\": true\n    },\n    \"filter\": {\n      \"type\": \"string\",\n      \"description\": \"Filter function name to limit replicated documents\",\n      \"example\": \"myapp/by_type\"\n    },\n    \"doc_ids\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of document IDs to replicate\"\n    }\n  },\n  \"required\": [\n    \"source\",\n    \"target\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-replication-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ReplicationRequest
---
