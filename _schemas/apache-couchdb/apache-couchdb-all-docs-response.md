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
