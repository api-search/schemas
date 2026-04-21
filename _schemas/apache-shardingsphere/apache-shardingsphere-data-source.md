---
description: Physical data source configuration
layout: schema
name: DataSource
properties_list:
- description: Data source name
  name: name
  type: string
- description: JDBC connection URL
  name: url
  type: string
- description: Database username
  name: username
  type: string
- description: Maximum connection pool size
  name: maxPoolSize
  type: integer
- description: Minimum connection pool size
  name: minPoolSize
  type: integer
- description: Connection pool type (HikariCP, etc.)
  name: type
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-data-source-schema.json
slug: apache-shardingsphere-data-source
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: DataSource
---
