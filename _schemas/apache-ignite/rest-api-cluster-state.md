---
description: Information about current cluster state.
layout: schema
name: ClusterState
properties_list:
- description: List of cluster management group nodes. These nodes are responsible for maintaining RAFT cluster topology.
  name: cmgNodes
  type: array
- description: List of metastorage nodes. These nodes are responsible for storing RAFT cluster metadata.
  name: msNodes
  type: array
- description: Version of Apache Ignite that the cluster was created on.
  name: igniteVersion
  type: string
- description: ''
  name: clusterTag
  type: object
- description: IDs the cluster had before.
  name: formerClusterIds
  type: array
provider_name: Apache Ignite
provider_slug: apache-ignite
schema_file: json-schema/rest-api-cluster-state-schema.json
slug: rest-api-cluster-state
tags:
- Caching
- Compute Grid
- Distributed Database
- In-Memory
- Open Source
- SQL
title: ClusterState
---
