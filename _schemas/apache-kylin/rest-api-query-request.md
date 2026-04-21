---
description: SQL query request
layout: schema
name: QueryRequest
properties_list:
- description: SQL query to execute
  name: sql
  type: string
- description: Project name to query
  name: project
  type: string
- description: Result offset for pagination
  name: offset
  type: integer
- description: Maximum number of results
  name: limit
  type: integer
- description: Accept partial results if query times out
  name: acceptPartial
  type: boolean
provider_name: Apache Kylin
provider_slug: apache-kylin
schema_file: json-schema/rest-api-query-request-schema.json
slug: rest-api-query-request
tags:
- Analytics
- Big Data
- Cube
- OLAP
- Open Source
- SQL
title: QueryRequest
---
