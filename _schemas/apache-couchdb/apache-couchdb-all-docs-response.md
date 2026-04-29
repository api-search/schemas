---
description: Response from _all_docs or bulk get
layout: schema
name: AllDocsResponse
properties_list:
- description: Total number of documents in the database
  name: total_rows
  type: integer
- description: Number of skipped rows
  name: offset
  type: integer
- description: ''
  name: rows
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-all-docs-response-schema.json
slug: apache-couchdb-all-docs-response
source_filename: apache-couchdb-all-docs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-all-docs-response-schema.json\",\n  \"title\": \"AllDocsResponse\",\n  \"description\": \"Response from _all_docs or bulk get\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_rows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of documents in the database\",\n      \"example\": 1250\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of skipped rows\",\n      \"example\": 0\n    },\n    \"rows\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"title\": \"DocRow\",\n        \"type\": \"object\",\n        \"description\": \"A row in an _all_docs response\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Document ID\",\n            \"\
  example\": \"doc001\"\n          },\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"Row key\",\n            \"example\": \"doc001\"\n          },\n          \"value\": {\n            \"type\": \"object\",\n            \"description\": \"Row value containing revision info\",\n            \"properties\": {\n              \"rev\": {\n                \"type\": \"string\",\n                \"example\": \"1-abc123\"\n              }\n            }\n          },\n          \"doc\": {\n            \"$ref\": \"#/components/schemas/Document\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-couchdb/refs/heads/main/json-schema/apache-couchdb-all-docs-response-schema.json
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: AllDocsResponse
---
