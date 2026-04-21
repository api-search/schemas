---
description: Cluster initialization configuration.
layout: schema
name: InitCommand
properties_list:
- description: A list of RAFT metastorage nodes.
  name: metaStorageNodes
  type: array
- description: A list of RAFT cluster management nodes.
  name: cmgNodes
  type: array
- description: The name of the cluster.
  name: clusterName
  type: string
- description: Cluster configuration in HOCON format.
  name: clusterConfiguration
  type: string
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-init-command-schema.json
slug: rest-api-init-command
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: InitCommand
---
