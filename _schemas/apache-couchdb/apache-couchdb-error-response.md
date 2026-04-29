---
description: Standard CouchDB error response
layout: schema
name: ErrorResponse
properties_list:
- description: Error type code
  name: error
  type: string
- description: Human-readable error description
  name: reason
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-error-response-schema.json
slug: apache-couchdb-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Standard CouchDB error response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"Error type code\",\n      \"example\": \"not_found\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\",\n      \"example\": \"Database does not exist.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-error-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ErrorResponse
---
