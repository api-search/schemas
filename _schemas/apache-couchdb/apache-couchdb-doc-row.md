---
description: A row in an _all_docs response
layout: schema
name: DocRow
properties_list:
- description: Document ID
  name: id
  type: string
- description: Row key
  name: key
  type: string
- description: Row value containing revision info
  name: value
  type: object
- description: A CouchDB document with system fields and user-defined fields
  name: doc
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-doc-row-schema.json
slug: apache-couchdb-doc-row
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DocRow
---
