---
description: Migrate nodes to new cluster.
layout: schema
name: MigrateRequest
properties_list:
- description: Names of the CMG node names.
  name: cmgNodes
  type: array
- description: Names of the Metastorage node names.
  name: metaStorageNodes
  type: array
- description: Ignite version.
  name: version
  type: string
- description: ID of the cluster.
  name: clusterId
  type: string
- description: Name of the cluster.
  name: clusterName
  type: string
- description: IDs the cluster had before. If CMG/Metastorage group were never repaired, this is null.
  name: formerClusterIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-migrate-request-schema.json
slug: rest-api-migrate-request
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: MigrateRequest
---
