---
description: Hive table partition
layout: schema
name: Partition
properties_list:
- description: Table name
  name: tableName
  type: string
- description: Database name
  name: dbName
  type: string
- description: Partition key values
  name: values
  type: array
- description: Partition HDFS location
  name: location
  type: string
- description: Approximate row count
  name: numRows
  type: integer
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-partition-schema.json
slug: hive-webhcat-partition
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Partition
---
