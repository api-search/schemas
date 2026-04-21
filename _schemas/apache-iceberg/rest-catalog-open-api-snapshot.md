---
description: Snapshot schema from Apache Iceberg REST Catalog API
layout: schema
name: Snapshot
properties_list:
- description: ''
  name: snapshot-id
  type: integer
- description: ''
  name: parent-snapshot-id
  type: integer
- description: ''
  name: sequence-number
  type: integer
- description: ''
  name: timestamp-ms
  type: integer
- description: Location of the snapshot's manifest list file
  name: manifest-list
  type: string
- description: The first _row_id assigned to the first row in the first data file in the first manifest
  name: first-row-id
  type: integer
- description: The upper bound of the number of rows with assigned row IDs
  name: added-rows
  type: integer
- description: ''
  name: summary
  type: object
- description: ''
  name: schema-id
  type: integer
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-snapshot-schema.json
slug: rest-catalog-open-api-snapshot
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: Snapshot
---
