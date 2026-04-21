---
description: Rest representation of sql query.
layout: schema
name: SqlQuery
properties_list:
- description: Sql query ID.
  name: id
  type: string
- description: Initiator node.
  name: node
  type: string
- description: Phase.
  name: phase
  type: string
- description: Type.
  name: type
  type: string
- description: Schema.
  name: schema
  type: string
- description: SQL statement.
  name: sql
  type: string
- description: Start time.
  name: startTime
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-sql-query-schema.json
slug: rest-api-sql-query
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: SqlQuery
---
