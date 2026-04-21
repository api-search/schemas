---
description: CouchDB server meta information
layout: schema
name: ServerInfo
properties_list:
- description: Always "Welcome"
  name: couchdb
  type: string
- description: CouchDB version number
  name: version
  type: string
- description: Git commit SHA of the build
  name: git_sha
  type: string
- description: Server-wide unique identifier
  name: uuid
  type: string
- description: ''
  name: vendor
  type: object
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-server-info-schema.json
slug: apache-couchdb-server-info
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ServerInfo
---
