---
description: Current session information
layout: schema
name: SessionInfo
properties_list:
- description: ''
  name: ok
  type: boolean
- description: ''
  name: userCtx
  type: object
- description: ''
  name: info
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-session-info-schema.json
slug: apache-couchdb-session-info
source_filename: apache-couchdb-session-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-session-info-schema.json\",\n  \"title\": \"SessionInfo\",\n  \"description\": \"Current session information\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ok\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"userCtx\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"example\": \"admin\"\n        },\n        \"roles\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"example\": [\n            \"_admin\"\n          ]\n        }\n      }\n    },\n    \"info\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"authentication_handlers\": {\n          \"type\": \"array\",\n          \"items\": {\n   \
  \         \"type\": \"string\"\n          },\n          \"example\": [\n            \"cookie\",\n            \"default\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-session-info-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: SessionInfo
---
