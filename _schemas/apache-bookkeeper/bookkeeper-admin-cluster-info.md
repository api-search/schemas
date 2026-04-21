---
description: BookKeeper cluster-wide status and bookie count information.
layout: schema
name: ClusterInfo
properties_list:
- description: Whether an auditor has been elected.
  name: auditorElected
  type: boolean
- description: Socket address of the elected auditor.
  name: auditorId
  type: string
- description: Whether any ledgers in the cluster are under-replicated.
  name: clusterUnderReplicated
  type: boolean
- description: Whether ledger replication is enabled.
  name: ledgerReplicationEnabled
  type: boolean
- description: Total number of bookies in the cluster.
  name: totalBookiesCount
  type: integer
- description: Number of bookies available for writes.
  name: writableBookiesCount
  type: integer
- description: Number of read-only bookies.
  name: readonlyBookiesCount
  type: integer
- description: Number of unavailable bookies.
  name: unavailableBookiesCount
  type: integer
provider_name: Apache BookKeeper
provider_slug: apache-bookkeeper
schema_file: json-schema/bookkeeper-admin-cluster-info-schema.json
slug: bookkeeper-admin-cluster-info
tags:
- Apache
- Distributed Systems
- Log Storage
- Open Source
- Storage
- Streaming
title: ClusterInfo
---
