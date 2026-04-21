---
description: Reset partitions configuration.
layout: schema
name: ResetPartitionsRequest
properties_list:
- description: Name of the zone to reset partitions of. Without quotes, case-sensitive.
  name: zoneName
  type: string
- description: IDs of partitions to reset. All if empty.
  name: partitionIds
  type: array
- description: Fully-qualified name of the table to reset partitions of. Without quotes, case-sensitive.
  name: tableName
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-reset-partitions-request-schema.json
slug: rest-api-reset-partitions-request
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ResetPartitionsRequest
---
