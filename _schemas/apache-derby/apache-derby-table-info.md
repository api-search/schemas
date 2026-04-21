---
description: Metadata about a table in an Apache Derby database, as returned by JDBC DatabaseMetaData.getTables().
layout: schema
name: TableInfo
properties_list:
- description: Name of the table.
  name: tableName
  type: string
- description: Schema (owner) of the table.
  name: tableSchema
  type: string
- description: Catalog of the table (always null in Derby).
  name: tableCatalog
  type: string
- description: Type of table object.
  name: tableType
  type: string
- description: Table comment if defined.
  name: remarks
  type: string
provider_name: Apache Derby
provider_slug: apache-derby
schema_file: json-schema/apache-derby-table-info-schema.json
slug: apache-derby-table-info
tags:
- Apache
- Database
- Embedded
- Java
- JDBC
- Open Source
- Relational
- SQL
title: TableInfo
---
