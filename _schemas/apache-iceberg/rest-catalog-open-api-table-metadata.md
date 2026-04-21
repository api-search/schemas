---
description: TableMetadata schema from Apache Iceberg REST Catalog API
layout: schema
name: TableMetadata
properties_list:
- description: ''
  name: format-version
  type: integer
- description: ''
  name: table-uuid
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: last-updated-ms
  type: integer
- description: A long higher than all assigned row IDs; the next snapshot's first-row-id.
  name: next-row-id
  type: integer
- description: ''
  name: properties
  type: object
- description: ''
  name: schemas
  type: array
- description: ''
  name: current-schema-id
  type: integer
- description: ''
  name: last-column-id
  type: integer
- description: ''
  name: partition-specs
  type: array
- description: ''
  name: default-spec-id
  type: integer
- description: ''
  name: last-partition-id
  type: integer
- description: ''
  name: sort-orders
  type: array
- description: ''
  name: default-sort-order-id
  type: integer
- description: ''
  name: encryption-keys
  type: array
- description: ''
  name: snapshots
  type: array
- description: ''
  name: refs
  type: object
- description: ''
  name: current-snapshot-id
  type: integer
- description: ''
  name: last-sequence-number
  type: integer
- description: ''
  name: snapshot-log
  type: object
- description: ''
  name: metadata-log
  type: object
- description: ''
  name: statistics
  type: array
- description: ''
  name: partition-statistics
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-table-metadata-schema.json
slug: rest-catalog-open-api-table-metadata
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: TableMetadata
---
