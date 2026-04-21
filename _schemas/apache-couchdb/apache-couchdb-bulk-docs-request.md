---
description: Request body for _bulk_docs
layout: schema
name: BulkDocsRequest
properties_list:
- description: Array of documents to create, update, or delete
  name: docs
  type: array
- description: If false, allow insertion of conflicting revisions (for replication)
  name: new_edits
  type: boolean
provider_name: Apache CouchDB
provider_slug: apache-couchdb
schema_file: json-schema/apache-couchdb-bulk-docs-request-schema.json
slug: apache-couchdb-bulk-docs-request
tags:
- Apache
- Database
- Document Store
- JSON
- NoSQL
- Open Source
- Replication
- REST
title: BulkDocsRequest
---
