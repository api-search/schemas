---
description: Reset cluster.
layout: schema
name: ResetClusterRequest
properties_list:
- description: Names of the proposed CMG nodes. Optional if the MG group is being repaired. If not specified, the current CMG nodes are used.
  name: cmgNodeNames
  type: array
- description: Number of nodes in the voting member set of the Metastorage RAFT group.
  name: metastorageReplicationFactor
  type: integer
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-reset-cluster-request-schema.json
slug: rest-api-reset-cluster-request
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ResetClusterRequest
---
