---
description: Hive table metadata
layout: schema
name: Table
properties_list:
- description: Table name
  name: tableName
  type: string
- description: Database name
  name: dbName
  type: string
- description: Table type (MANAGED_TABLE, EXTERNAL_TABLE, VIRTUAL_VIEW)
  name: tableType
  type: string
- description: Table description
  name: comment
  type: string
- description: HDFS data location
  name: location
  type: string
- description: Input format class
  name: inputFormat
  type: string
- description: Output format class
  name: outputFormat
  type: string
- description: Approximate number of rows
  name: numRows
  type: integer
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-table-schema.json
slug: hive-webhcat-table
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Table
---
