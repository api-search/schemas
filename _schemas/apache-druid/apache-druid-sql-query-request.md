---
description: Request body for the Apache Druid SQL query API (POST /druid/v2/sql).
layout: schema
name: SqlQueryRequest
properties_list:
- description: SQL query string to execute.
  name: query
  type: string
- description: Format for the query results.
  name: resultFormat
  type: string
- description: Whether to return column names in the first row (for array/objectLines formats).
  name: header
  type: boolean
- description: Whether to include column data types in a header row.
  name: typesHeader
  type: boolean
- description: Whether to include SQL type names in a header row.
  name: sqlTypesHeader
  type: boolean
- description: Query context parameters for controlling execution behavior.
  name: context
  type: object
- description: Parameterized query values.
  name: parameters
  type: array
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-sql-query-request-schema.json
slug: apache-druid-sql-query-request
tags:
- Analytics
- Apache
- Database
- Kafka
- OLAP
- Open Source
- Real-Time
- SQL
- Time Series
title: SqlQueryRequest
---
