---
description: Request to create a Mango index
layout: schema
name: CreateIndexRequest
properties_list:
- description: Index definition
  name: index
  type: object
- description: Design document name to use for the index
  name: ddoc
  type: string
- description: Index name
  name: name
  type: string
- description: Index type
  name: type
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-create-index-request-schema.json
slug: apache-couchdb-create-index-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-create-index-request-schema.json\",\n  \"title\": \"CreateIndexRequest\",\n  \"description\": \"Request to create a Mango index\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"object\",\n      \"description\": \"Index definition\",\n      \"properties\": {\n        \"fields\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"oneOf\": [\n              {\n                \"type\": \"string\"\n              },\n              {\n                \"type\": \"object\"\n              }\n            ]\n          },\n          \"description\": \"Fields to index\"\n        }\n      }\n    },\n    \"ddoc\": {\n      \"type\": \"string\",\n      \"description\": \"Design document name to use for the index\",\n      \"example\": \"idx-status-type\"\
  \n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Index name\",\n      \"example\": \"idx-status-type\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Index type\",\n      \"enum\": [\n        \"json\",\n        \"text\"\n      ],\n      \"default\": \"json\",\n      \"example\": \"json\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-create-index-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: CreateIndexRequest
---
