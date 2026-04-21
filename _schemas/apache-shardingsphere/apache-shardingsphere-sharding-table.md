---
description: Sharding configuration for a logical table
layout: schema
name: ShardingTable
properties_list:
- description: Logical table name
  name: logicTable
  type: string
- description: Actual data nodes expression (e.g. ds${0..1}.orders${0..3})
  name: actualDataNodes
  type: string
- description: ''
  name: databaseStrategy
  type: object
- description: ''
  name: tableStrategy
  type: object
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-table-schema.json
slug: apache-shardingsphere-sharding-table
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingTable
---
