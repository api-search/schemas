---
description: Helix cluster configuration and state
layout: schema
name: Cluster
properties_list:
- description: Cluster name
  name: id
  type: string
- description: Active controller node
  name: controller
  type: string
- description: Whether the cluster is paused
  name: paused
  type: boolean
- description: List of disabled instances
  name: disabledInstances
  type: array
- description: List of live instances
  name: liveInstances
  type: array
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-cluster-schema.json
slug: helix-rest-cluster
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Cluster
---
