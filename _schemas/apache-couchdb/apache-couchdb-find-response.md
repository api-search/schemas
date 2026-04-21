---
description: Mango query results
layout: schema
name: FindResponse
properties_list:
- description: Array of matching documents
  name: docs
  type: array
- description: Bookmark for retrieving the next set of results
  name: bookmark
  type: string
- description: Warning if query is not optimally indexed
  name: warning
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-find-response-schema.json
slug: apache-couchdb-find-response
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: FindResponse
---
