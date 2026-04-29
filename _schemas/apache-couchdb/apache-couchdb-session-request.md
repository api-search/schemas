---
description: Authentication credentials for session creation
layout: schema
name: SessionRequest
properties_list:
- description: CouchDB username
  name: name
  type: string
- description: CouchDB password
  name: password
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-session-request-schema.json
slug: apache-couchdb-session-request
source_filename: apache-couchdb-session-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-session-request-schema.json\",\n  \"title\": \"SessionRequest\",\n  \"description\": \"Authentication credentials for session creation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"CouchDB username\",\n      \"example\": \"admin\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"CouchDB password\",\n      \"example\": \"secretpassword\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"password\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-session-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: SessionRequest
---
