---
description: Request body for POST _all_docs with specific keys
layout: schema
name: KeysRequest
properties_list:
- description: Array of document IDs to retrieve
  name: keys
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-keys-request-schema.json
slug: apache-couchdb-keys-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-keys-request-schema.json\",\n  \"title\": \"KeysRequest\",\n  \"description\": \"Request body for POST _all_docs with specific keys\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Array of document IDs to retrieve\",\n      \"example\": [\n        \"doc001\",\n        \"doc002\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-keys-request-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: KeysRequest
---
