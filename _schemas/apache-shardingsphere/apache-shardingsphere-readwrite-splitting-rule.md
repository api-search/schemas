---
description: Read-write splitting configuration
layout: schema
name: ReadwriteSplittingRule
properties_list:
- description: Rule name
  name: name
  type: string
- description: Primary/write data source
  name: writeDataSourceName
  type: string
- description: Replica/read data sources
  name: readDataSourceNames
  type: array
- description: Load balancer algorithm name
  name: loadBalancerName
  type: string
provider_name: Apache ShardingSphere
provider_slug: apache-shardingsphere
schema_file: json-schema/apache-shardingsphere-readwrite-splitting-rule-schema.json
slug: apache-shardingsphere-readwrite-splitting-rule
tags:
- Database
- Distributed SQL
- Read-Write Splitting
- Sharding
- SQL
- Apache
- Open Source
title: ReadwriteSplittingRule
---
