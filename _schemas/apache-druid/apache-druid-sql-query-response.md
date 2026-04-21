---
description: Response from the Apache Druid SQL API with query results and metadata.
layout: schema
name: SqlQueryResponse
properties_list:
- description: Unique ID assigned to this query.
  name: queryId
  type: string
- description: Column names in result order.
  name: columns
  type: array
- description: Column Druid types.
  name: columnTypes
  type: array
- description: Column SQL types.
  name: sqlTypes
  type: array
- description: Query result rows (format depends on resultFormat).
  name: results
  type: array
provider_name: Apache Druid
provider_slug: apache-druid
schema_file: json-schema/apache-druid-sql-query-response-schema.json
slug: apache-druid-sql-query-response
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
title: SqlQueryResponse
---
