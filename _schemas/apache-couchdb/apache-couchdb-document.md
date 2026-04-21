---
description: A CouchDB document with system fields and user-defined fields
layout: schema
name: Document
properties_list:
- description: Document ID
  name: _id
  type: string
- description: Current revision ID (major-hash format)
  name: _rev
  type: string
- description: Present and true for deleted (tombstone) documents
  name: _deleted
  type: boolean
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-document-schema.json
slug: apache-couchdb-document
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: Document
---
