---
description: Database changes feed response
layout: schema
name: ChangesResponse
properties_list:
- description: Last sequence number in this response
  name: last_seq
  type: string
- description: Number of changes still pending
  name: pending
  type: integer
- description: ''
  name: results
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-changes-response-schema.json
slug: apache-couchdb-changes-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-changes-response-schema.json\",\n  \"title\": \"ChangesResponse\",\n  \"description\": \"Database changes feed response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"last_seq\": {\n      \"type\": \"string\",\n      \"description\": \"Last sequence number in this response\",\n      \"example\": \"5000-abc123\"\n    },\n    \"pending\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of changes still pending\",\n      \"example\": 0\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"ChangeRow\",\n        \"type\": \"object\",\n        \"description\": \"A single change record in the changes feed\",\n        \"properties\": {\n          \"seq\": {\n            \"type\": \"string\",\n            \"description\": \"Update\
  \ sequence number\",\n            \"example\": \"5000-abc123\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Document ID that was changed\",\n            \"example\": \"doc001\"\n          },\n          \"changes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"rev\": {\n                  \"type\": \"string\",\n                  \"example\": \"2-def456\"\n                }\n              }\n            }\n          },\n          \"deleted\": {\n            \"type\": \"boolean\",\n            \"description\": \"True if this change is a deletion\",\n            \"example\": false\n          },\n          \"doc\": {\n            \"$ref\": \"#/components/schemas/Document\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-changes-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ChangesResponse
---
