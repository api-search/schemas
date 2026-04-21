---
description: Reset zone partitions configuration.
layout: schema
name: ResetZonePartitionsRequest
properties_list:
- description: Name of the zone to reset partitions of. Without quotes, case-sensitive.
  name: zoneName
  type: string
- description: IDs of partitions to reset. All if empty.
  name: partitionIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-reset-zone-partitions-request-schema.json
slug: rest-api-reset-zone-partitions-request
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ResetZonePartitionsRequest
---
