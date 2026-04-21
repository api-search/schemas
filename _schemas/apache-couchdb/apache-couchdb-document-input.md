---
description: Input for creating or updating a CouchDB document
layout: schema
name: DocumentInput
properties_list:
- description: Optional document ID (auto-generated if omitted for POST)
  name: _id
  type: string
- description: Required for updates — current revision ID
  name: _rev
  type: string
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-document-input-schema.json
slug: apache-couchdb-document-input
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: DocumentInput
---
