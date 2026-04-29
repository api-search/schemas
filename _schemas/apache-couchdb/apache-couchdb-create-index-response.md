---
description: Response from creating a Mango index
layout: schema
name: CreateIndexResponse
properties_list:
- description: created or exists
  name: result
  type: string
- description: Design document ID
  name: id
  type: string
- description: Index name
  name: name
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-create-index-response-schema.json
slug: apache-couchdb-create-index-response
source_filename: apache-couchdb-create-index-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-create-index-response-schema.json\",\n  \"title\": \"CreateIndexResponse\",\n  \"description\": \"Response from creating a Mango index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"created or exists\",\n      \"enum\": [\n        \"created\",\n        \"exists\"\n      ],\n      \"example\": \"created\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Design document ID\",\n      \"example\": \"_design/idx-status-type\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Index name\",\n      \"example\": \"idx-status-type\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-create-index-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: CreateIndexResponse
---
