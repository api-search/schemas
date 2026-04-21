---
description: Schema definition for an Apache Doris table, describing columns, keys, and partitioning.
layout: schema
name: TableSchema
properties_list:
- description: Name of the table.
  name: tableName
  type: string
- description: Database containing the table.
  name: databaseName
  type: string
- description: Data model of the table.
  name: tableType
  type: string
- description: Key model for the table.
  name: keyType
  type: string
- description: List of column definitions.
  name: columns
  type: array
- description: Table comment.
  name: comment
  type: string
- description: Number of data replicas.
  name: replicationNum
  type: integer
provider_name: Apache Doris
provider_slug: apache-doris
schema_file: json-schema/apache-doris-table-schema-schema.json
slug: apache-doris-table-schema
tags:
- Analytics
- Apache
- Database
- Lakehouse
- MPP
- OLAP
- Open Source
- Real-Time
- SQL
title: TableSchema
---
