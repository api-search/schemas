---
description: Simple success acknowledgement
layout: schema
name: OkResponse
properties_list:
- description: ''
  name: ok
  type: boolean
- description: Username (for session responses)
  name: name
  type: string
- description: ''
  name: roles
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-ok-response-schema.json
slug: apache-couchdb-ok-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-ok-response-schema.json\",\n  \"title\": \"OkResponse\",\n  \"description\": \"Simple success acknowledgement\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Username (for session responses)\",\n      \"example\": \"admin\"\n    },\n    \"roles\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"_admin\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-ok-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: OkResponse
---
