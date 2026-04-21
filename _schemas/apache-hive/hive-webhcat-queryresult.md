---
description: Result of a WebHCat DDL or DML operation
layout: schema
name: QueryResult
properties_list:
- description: HTTP status code
  name: status
  type: integer
- description: Result schema as JSON string
  name: schema
  type: string
- description: Result rows
  name: rows
  type: array
- description: Active database
  name: database
  type: string
provider_name: Apache Hive
provider_slug: apache-hive
schema_file: json-schema/hive-webhcat-queryresult-schema.json
slug: hive-webhcat-queryresult
tags:
- Apache
- Big Data
- Data Warehouse
- ETL
- Hadoop
- Open Source
- SQL
title: QueryResult
---
