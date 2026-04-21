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
