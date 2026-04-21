---
description: Hudi query configuration for incremental or snapshot queries
layout: schema
name: QueryConfig
properties_list:
- description: Query type (SNAPSHOT, INCREMENTAL, READ_OPTIMIZED)
  name: queryType
  type: string
- description: Start instant for incremental queries
  name: beginInstantTime
  type: string
- description: End instant for incremental queries
  name: endInstantTime
  type: string
- description: Maximum commits to include in incremental query
  name: maxCommits
  type: integer
provider_name: Apache Hudi
provider_slug: apache-hudi
schema_file: json-schema/hudi-queryconfig-schema.json
slug: hudi-queryconfig
tags:
- ACID
- Apache
- Big Data
- Data Lake
- Incremental Processing
- Lakehouse
- Open Source
title: QueryConfig
---
