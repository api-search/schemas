---
description: List of Mango indexes for a database
layout: schema
name: IndexesResponse
properties_list:
- description: Number of indexes
  name: total_rows
  type: integer
- description: ''
  name: indexes
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-indexes-response-schema.json
slug: apache-couchdb-indexes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-indexes-response-schema.json\",\n  \"title\": \"IndexesResponse\",\n  \"description\": \"List of Mango indexes for a database\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of indexes\",\n      \"example\": 2\n    },\n    \"indexes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ddoc\": {\n            \"type\": \"string\",\n            \"example\": \"_design/idx-status\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"idx-status\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"json\"\n          },\n          \"def\": {\n   \
  \         \"type\": \"object\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-indexes-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: IndexesResponse
---
