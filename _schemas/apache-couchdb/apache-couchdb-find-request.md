---
description: Mango query request
layout: schema
name: FindRequest
properties_list:
- description: Mango selector (JSON query expression)
  name: selector
  type: object
- description: Fields to return in results
  name: fields
  type: array
- description: Maximum number of results
  name: limit
  type: integer
- description: Number of results to skip
  name: skip
  type: integer
- description: Sort order specification
  name: sort
  type: array
- description: Bookmark for pagination from previous query
  name: bookmark
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-find-request-schema.json
slug: apache-couchdb-find-request
source_filename: apache-couchdb-find-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-find-request-schema.json\",\n  \"title\": \"FindRequest\",\n  \"description\": \"Mango query request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"selector\": {\n      \"type\": \"object\",\n      \"description\": \"Mango selector (JSON query expression)\",\n      \"example\": {\n        \"type\": \"product\",\n        \"status\": \"active\"\n      }\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Fields to return in results\",\n      \"example\": [\n        \"_id\",\n        \"name\"\n      ]\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of results\",\n      \"default\": 25,\n      \"example\": 25\n    },\n    \"skip\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Number of results to skip\",\n      \"default\": 0,\n      \"example\": 0\n    },\n    \"sort\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"Sort order specification\",\n      \"example\": [\n        {\n          \"name\": \"asc\"\n        }\n      ]\n    },\n    \"bookmark\": {\n      \"type\": \"string\",\n      \"description\": \"Bookmark for pagination from previous query\",\n      \"example\": \"g1AAAABleJzLYWBg\"\n    }\n  },\n  \"required\": [\n    \"selector\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-find-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: FindRequest
---
