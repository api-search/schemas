---
description: Hive database (schema) in the metastore
layout: schema
name: Database
properties_list:
- description: Database name
  name: name
  type: string
- description: Database description
  name: comment
  type: string
- description: HDFS location URI
  name: location
  type: string
- description: Owner of the database
  name: ownerName
  type: string
- description: Owner type (USER or ROLE)
  name: ownerType
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-database-schema.json
slug: hive-webhcat-database
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: Database
---
