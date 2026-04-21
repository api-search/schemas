---
description: A single change record in the changes feed
layout: schema
name: ChangeRow
properties_list:
- description: Update sequence number
  name: seq
  type: string
- description: Document ID that was changed
  name: id
  type: string
- description: ''
  name: changes
  type: array
- description: True if this change is a deletion
  name: deleted
  type: boolean
- description: A CouchDB document with system fields and user-defined fields
  name: doc
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-change-row-schema.json
slug: apache-couchdb-change-row
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ChangeRow
---
