---
description: restart partitions configuration.
layout: schema
name: RestartPartitionsRequest
properties_list:
- description: Names specifying nodes to restart partitions. Case-sensitive. If empty/omitted, partitions on all nodes are restarted.
  name: nodeNames
  type: array
- description: Name of the zone to restart partitions of. Without quotes, case-sensitive.
  name: zoneName
  type: string
- description: IDs of partitions to restart. If empty/omitted, all partitions will be restarted.
  name: partitionIds
  type: array
- description: Fully-qualified name of the table to restart partitions of.
  name: tableName
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-restart-partitions-request-schema.json
slug: rest-api-restart-partitions-request
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: RestartPartitionsRequest
---
