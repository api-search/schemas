---
description: Sharding strategy definition
layout: schema
name: ShardingStrategy
properties_list:
- description: Strategy type
  name: type
  type: string
- description: Column used for sharding
  name: shardingColumn
  type: string
- description: Sharding algorithm reference
  name: shardingAlgorithmName
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-sharding-strategy-schema.json
slug: apache-shardingsphere-sharding-strategy
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ShardingStrategy
---
