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
