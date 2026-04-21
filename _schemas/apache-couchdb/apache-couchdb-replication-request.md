---
description: Replication task parameters
layout: schema
name: ReplicationRequest
properties_list:
- description: Source database URL or name
  name: source
  type: string
- description: Target database URL or name
  name: target
  type: string
- description: Keep the replication running continuously
  name: continuous
  type: boolean
- description: Create the target database if it does not exist
  name: create_target
  type: boolean
- description: Filter function name to limit replicated documents
  name: filter
  type: string
- description: List of document IDs to replicate
  name: doc_ids
  type: array
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-replication-request-schema.json
slug: apache-couchdb-replication-request
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: ReplicationRequest
---
