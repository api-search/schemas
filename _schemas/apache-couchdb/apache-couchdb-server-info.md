---
description: CouchDB server meta information
layout: schema
name: ServerInfo
properties_list:
- description: Always "Welcome"
  name: couchdb
  type: string
- description: CouchDB version number
  name: version
  type: string
- description: Git commit SHA of the build
  name: git_sha
  type: string
- description: Server-wide unique identifier
  name: uuid
  type: string
- description: ''
  name: vendor
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-server-info-schema.json
slug: apache-couchdb-server-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-server-info-schema.json\",\n  \"title\": \"ServerInfo\",\n  \"description\": \"CouchDB server meta information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"couchdb\": {\n      \"type\": \"string\",\n      \"description\": \"Always \\\"Welcome\\\"\",\n      \"example\": \"Welcome\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"CouchDB version number\",\n      \"example\": \"3.5.1\"\n    },\n    \"git_sha\": {\n      \"type\": \"string\",\n      \"description\": \"Git commit SHA of the build\",\n      \"example\": \"abc1234\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Server-wide unique identifier\",\n      \"example\": \"a1b2c3d4e5f6a7b8c9d0e1f2a3b4c5d6\"\n    },\n    \"vendor\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"The Apache Software Foundation\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-server-info-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ServerInfo
---
