---
description: SQL query response
layout: schema
name: QueryResponse
properties_list:
- description: Result column metadata
  name: columnMetas
  type: array
- description: Query result rows
  name: results
  type: array
- description: ''
  name: queryId
  type: string
- description: ''
  name: isException
  type: boolean
- description: ''
  name: exceptionMessage
  type: string
- description: Query duration in milliseconds
  name: duration
  type: integer
- description: ''
  name: totalScanCount
  type: integer
- description: ''
  name: totalScanBytes
  type: integer
- description: ''
  name: hitExceptionCache
  type: boolean
- description: ''
  name: storageCacheUsed
  type: boolean
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-query-response-schema.json
slug: rest-api-query-response
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: QueryResponse
---
