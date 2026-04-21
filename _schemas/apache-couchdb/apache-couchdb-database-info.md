---
description: Information about a CouchDB database
layout: schema
name: DatabaseInfo
properties_list:
- description: Database name
  name: db_name
  type: string
- description: Number of non-deleted documents
  name: doc_count
  type: integer
- description: Number of deleted documents (tombstones)
  name: doc_del_count
  type: integer
- description: Current update sequence
  name: update_seq
  type: string
- description: ''
  name: sizes
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-database-info-schema.json
slug: apache-couchdb-database-info
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DatabaseInfo
---
